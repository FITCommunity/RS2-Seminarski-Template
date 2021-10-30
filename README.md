# RS2-Seminarski-Template

## .NET 3.1 vs .NET 5

Defaultno template radi za .NET 5, u slučaju da koristite .NET 3.1 u `docker-compose.yml` treba promijeniti vrijednost za `dockerfile` sa `Dockerfile.NET5` na `Dockerfile.NET3`

```diff
 build:
     context: .
-    dockerfile: Dockerfile.NET5
+    dockerfile: Dockerfile.NET3
```
