Environment file:
```
FLOW_VERSION=2024.2.0
REPOSITORY=bitvis.jfrog.io/docker-release
TZ=Europe/Stockholm
JAVA_OPTS=-Xmn100m -Xmx4096m -XX:MinHeapFreeRatio=20 -XX:MaxHeapFreeRatio=40 -XX:HeapDumpPath=/data
HOST_IP=
PREFIX=
DATABASE_USER=flow
DATABASE_PASSWORD=
DATABASE_MASTER_PASSWORD=
FLOW_DOMAIN=flow.test.kurbit.se
ACCESS_DOMAIN=access.test.kurbit.se
METABASE_DOMAIN=metabase.test.kurbit.se
PORTAL_DOMAIN=portal.test.kurbit.se
```
For traefik to handle letsencrypt certificates via Azure
```
AZURE_CLIENT_SECRET=
AZURE_TENANT_ID=
AZURE_SUBSCRIPTION_ID=
AZURE_RESOURCE_GROUP=
AZURE_CLIENT_ID=
```
Start with docker compose -f flow.yml -f monitoring.yml up -d or docker compose -f access.yml up -d
