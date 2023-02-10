# API Server
Register users and invoke the transaction through API Server

## Registering User - API Server 1
1. Go to 10.api/src folder

## Transaction and Query Function - API Server 2
1. Transaction route
2. still src folder appl.js

## Creating Connection Profile
1. Open the terminal (MAC)
2. Check prerequiste folder - cpp.sh
3. move to the folder

```bash
cd nfs_clientshare
```
4. ./scripts/ccp.sh
5. ls connection-profile
6. We can find ccp-template.json and ymal / connection-org1.json and yaml
7. cat connection-profile/connection-org1.json

## Overriding Fabric CA Default Configuration

1. 10.api folder
2. Make k8 folder
3. make configmap.yaml
4. check npm package - fabric-ca-client / default.json file
5. move to the folder /hlf-kubernetes/10.api/k8 on CLI (MAC)
6. kubectl apply -f .

## Creating API Server Deployment

1. 10.api/k8 folder
2. create api.yaml
3. create Dockerfile
4. visit Dockerhub
5. create repository sseongha11/api
6. (MAC Terminal) cd hlf-kubernetes/10.pi/src
7. docker build -t sseongha11/api:1.0 .
8. docker push sseongha11/api:1.0
9. Verify the tag page (Dockerhub)

## Starting API Server
1. move to the directory (10.api/k8)
2. kubectl apply -f api.yaml
3. kubectl get deployment.apps
3. Visit Lens IDE