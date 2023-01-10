# Flutter Chat App using Node.JS, Socket.io and Redis

## Overview

https://user-images.githubusercontent.com/1321179/211640969-32b64a0c-de69-4b5a-91b2-27b822bdba60.mp4

This repo contain the code for a Flutter chat application with Node.JS, Socket.io and Redis backend.

To learn how this app was built you can read the blog post: [Flutter Chat App without Firebase using Node.JS, Socket.io and Redis](https://deadsimplechat.com/blog/flutter-chat-app-without-firebase/)

## Directory Structure

```
chat-backend/ -> Contains Node.JS Backend
custom_chat_app/ -> Contains Flutter Chat App
```

## Running the backend

To run the backend you need to have Redis and Node.JS Installed.

If you have docker you can launch the Redis docker by:

```
docker pull redis
```

```
docker run -d -p 6379:6379 --name myredis redis
```

The cd into the project directory

```
cd chat-backend
```

Install dependency

```
npm install
```

Start the server

```
node index.js
```

## Running the Flutter App

Make sure you have the Flutter Cli installed

The edit `custom_chat_app/lib/main.dart` line #67 and replace `http://192.168.1.134:3000` with IP address of your computer.

`cd` into the project directory

```
cd custom_chat_app
```

Launch the flutter app using the run command.

```
flutter run
```
