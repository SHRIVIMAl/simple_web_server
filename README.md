# EX01 Developing a Simple Webserver

# Date:07.12.2024
# AIM:
To develop a simple webserver to serve html pages and display the configuration details of laptop.

# DESIGN STEPS:
## Step 1:
HTML content creation.

## Step 2:
Design of webserver workflow.

## Step 3:
Implementation using Python code.

## Step 4:
Serving the HTML pages.

## Step 5:
Testing the webserver.

# PROGRAM:
```
""" from http.server import HTTPServer,BaseHTTPRequestHandler
content=''' <!doctype html>
<title> My Web Server</title>

        </table>
'''
class MyServer(BaseHTTPRequestHandler): def do_GET(self): print("Get request
received...") self.send_response(200) self.send_header("content-type", "text/html")
self.end_headers() self.wfile.write(content.encode())
print("This is my webserver") server_address =('',8000) httpd =
HTTPServer(server_address,MyServer) httpd.serve_forever() """
```
            
# OUTPUT:
![357670fc-4851-4b95-9c44-e834bd79fd7b](https://github.com/user-attachments/assets/48d4c1bd-746a-41a3-8103-392f30421f28)

# RESULT:
The program for implementing simple webserver is executed successfully.
![ff5bd7c8-c90a-4fcb-ac28-19d7ed508ea6](https://github.com/user-attachments/assets/60258497-2a16-4154-8616-754509d716d5)
