# 🌟 Golang Web Server 🌟
Welcome to the Golang Web Server project! This project showcases my learning journey with Go by implementing a basic web server that serves static files and handles form submissions. 🚀

## 📜 Overview
This project consists of a web server written in Go. It demonstrates essential concepts such as routing, handling HTTP requests, and serving static files.

## 🗺️ Flowchart
![flow](https://github.com/VastavNissan/golang-web-server/assets/88283180/ffcfb3b2-c36d-453e-9a76-e21e9551c186)

## 🖥️ Project Structure

### main.go
- Initializes the server and routes.
- Handles HTTP requests.
- Serves static files.
### static/
- Contains index.html for serving static content.
- Contains form.html for form submission.

## 📋 Code Explanation
### main.go

- **FileServer**: Serves static files from the `./static` directory.
- **Handlers**:
  - **formHandler**: Processes form submissions, extracts `name` and `address`, and responds with the form data.
  - **helloHandler**: Responds with "hello!" when `/hello` is requested.
- **Server Initialization**: Starts the server on port 8080.

### static/index.html

- Simple static webpage displaying "Static website".

### static/form.html

- Form submission page with fields for `name` and `address`.

## 🌟 Highlights
- **Routing**: Used `http.Handle` and `http.HandleFunc` for routing.
- **Request Parsing**: Used `r.ParseForm` to parse form data.
- **HTTP Methods**: Demonstrated handling of GET and POST requests.
- **Serving Static Files**: Used `http.FileServer` to serve static content.

## 📚 Go Concepts Used
- **HTTP Routing**: Creating different routes to handle various endpoints.
- **Form Handling**: Parsing and processing form data from POST requests.
- **Static File Serving**: Serving static files using `http.FileServer`.
- **Error Handling**: Managing errors effectively using Go's error handling mechanisms.
