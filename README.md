# RS2-Seminarski-Template

## Struktura

U slučaju da ne koristite "standardnu" strukturu sa RS2 potrebno je promijeniti `paths` u `docker-build.yml`, `paths` `flutter-build.yml` i prvu liniju u `run` u `flutter-build.yml`

```
.
├───Mobile
├───Model
├───WebAPI
└───WinUI
```

## .NET 3.1 vs .NET 5

Defaultno template radi za .NET 5, u slučaju da koristite .NET 3.1 u `docker-compose.yml` treba promijeniti vrijednost za `dockerfile` sa `Dockerfile.NET5` na `Dockerfile.NET3`

```diff
 build:
     context: .
-    dockerfile: Dockerfile.NET5
+    dockerfile: Dockerfile.NET3
```
