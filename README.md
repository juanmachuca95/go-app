## Deploy Go-APP with Google Cloud 

Link: https://cloud.google.com/appengine/docs/standard/go/building-app

1. Debes tener instalado el cliente de google cloud 

2. Luego crear un directorio de trabajo: 

```zsh
mkdir go-app
cd go-app
```

3. Crear un archivo app.yaml y escribir:

```yaml
runtime: go116 # el último soportado hasta el momento por google -- si tienes una version superior fallará
```

4. Programar un mini servicio de prueba

5. Realizar el deploy: Nota debes estar situado en la raiz del proyecto. 

```gcloud
gcloud app deploy
```

6. Todo listo, si todo esta okay deberias ver la url de tu servicio además del comando ```gcloud app browser``` para lanzar el navegador con la ruta de tu api.