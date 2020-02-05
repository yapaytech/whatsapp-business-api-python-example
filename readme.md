# Yapaytech - WhatsApp Business Bot Example

> A simple python bot for WhatsApp Business Api

[Our Website](https://yapaytech.com/products/whatsapp-business-api/) • [Facebook WhatsApp Documentations](https://developers.facebook.com/docs/whatsapp/api/reference)

- In this example we echo the text messages back to user.
- We use ngrok to create temporary https reverse proxy so whatsapp can reach our demo api.
- Because ngrok public url changes everytime we also change webhook settings in our instance at boot. This should not be used like this in production environments.

# Installation

### Installing python libraries

`pip install -r requirements.txt`

### Configure Tokens

You need to change INSTANCE_URL, API_KEY and ADMIN_API_KEY values in app.py file.

# Start The Api

Tested with python v3.8.1

## Mac/Linux

```
export FLASK_APP=app.py
flask run --host 0.0.0.0 --port 9000 --no-debugger --no-reload
```

## Windows Cmd

```
set FLASK_APP=app.py
flask run --host 0.0.0.0 --port 9000 --no-debugger --no-reload
```

## Windows PowerShell

```
$env:FLASK_APP = "app.py"
flask run --host 0.0.0.0 --port 9000 --no-debugger --no-reload
```
