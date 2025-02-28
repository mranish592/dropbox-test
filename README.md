## Dropbox Test

### Description
The goal of the project is to implement a simplified Dropbox like Product, where users
can upload and download files through a Web Application.

### Primary Requirements 
- WebApp
- Allow users to upload ```/upload```
- Allow users to download ```/download```
- Users should be able to login and signup

### Constraints
- RESTful APIs
- Persistent storage for data (files) and metatdata
- Web Application using front framework (React)

### Backend requirements
- /upload - Upload a file
- /list - list of all files (metadata, preview)
- /download - download a file

### Frontend requirements
- User home page: All files belonging to the user should be listed here.
- User should be able to add restrictions on types of files that will be supported for uploads. (need clarity, on whether the user or the front end can add this)
- Upload button: to upload a new file
- Click on file for preview: should ope the file contents in a new page (Can be restricted to well-known formats: txt, jpg, png, json, etc)
- login and signup page and autmatic routing based on the login status of the user.
  
## Technologies
- Langauge and framework: Java - Springboot, Python – Django / Fast API, NodeJS – Express (We will go ahead with vert.x with Kotlin, and springboot as backup
- DB - SQLLite, Mysql, Postgres or MongoDB. (need to decide, for storing files and for storing metadata and user login info)
- File Storage: AWS s3, Azure storage blob storage, local file system (think of good potential blob storage options. privde adapter/strategy for all)
- Use Docker ontainser for all DBMs and any exteral service that you're running.

## Secondary Requirements/Features
- OAuth google login, github login, login with email
- sort by created data, modified date
- drag and drop files onto a highlighted area (frontend-only)
- search your files
- load low resolution preview
- delete feature
- upload folders
- create folders and organise content
- duplicate file deteaction by hasing the name and the contents of the file
- 
