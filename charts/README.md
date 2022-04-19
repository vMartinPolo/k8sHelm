## Depurar en local

Podemos ejecutar el comando:

```bash
helm install --debug --dry-run --values .\eoloserver\values.yaml release-name .\eoloserver | code -
```
NOTA: Se nos abrira un tab em el VSCode donde podremos buscar lo que corresponda. Cuando cerremos ese tab la terminal nos volverá a responder. 

## Instalar una release

```bash
helm install release01 . --values=values.yaml
```
NOTA: El chart está implementado para poder instalar dos releases distintas en el mismo namespace.

## Actualizar una release

```bash
helm upgrade --install release01 . --values=values.yaml
```

## ArtifactHub
Puedes descargar el chart de Helm de: https://artifacthub.io/packages/helm/ihuertas2021-vmartinp2021-helm/eoloserver
