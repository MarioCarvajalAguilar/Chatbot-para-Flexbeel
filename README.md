# Chatbot-para-Flexbeel
Proyecto Chatbot para la empresa Flexbeel destinado a ayudar con el proceso de facturacion.

## Configuración inicial:
Este repositorio actualmente contiene los archivos listos.

Tiene que tener instalado el programa Git Bash, en este se deben de ejecutar los siguientes comandos. se encuentra en esta pagina
https://git-scm.com/downloads


primero ingresar a la carpeta del proyecto y crear un entorno virtual
```
$ cd chatbot-deployment
$ python3 -m venv venv
$ . venv/Scripts/activate

Instalar dependencias
```
$ (venv) pip install Flask torch torchvision nltk
```
Instalar el paquete nltk
```
$ (venv) python
>>> import nltk
>>> nltk.download('punkt')
```
Modifique `intents.json` con diferentes intentos y respuestas para su Chatbot

Correr
```
$ (venv) python train.py
```
Esto volcará el archivo data.pth. y luego corre
el siguiente comando para probarlo en la consola.
```
$ (venv) python chat.py
```
Posteriormente para ejecutarlo en el entorno web, tiene que ejecutra el archivo app.py, este le otorgara una direccion de hostlocal. al abrirla en un explorador deberia poder visualizar el chatbot.
```

