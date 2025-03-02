## Dropbox Test

### Description
The goal of the project is to implement a simplified Dropbox like Product, where users
can upload and download files through a Web Application.

### Primary Requirements 
- WebApp
- Allow users to upload ```/upload```
- Allow users to download ```/download```
- Users should be able to ```/login``` and ```/signup```

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
  
### Technologies
- Langauge and framework: Java - Springboot, Python – Django / Fast API, NodeJS – Express (We will go ahead with vert.x with Kotlin, and springboot as backup
- DB - SQLLite, Mysql, Postgres or MongoDB. (need to decide, for storing files and for storing metadata and user login info)
- File Storage: AWS s3, Azure storage blob storage, local file system (think of good potential blob storage options. provide adapter/strategy for all)
- Use Docker ontainser for all DBMs and any exteral service that you're running.

### Technology and framework
- Language: Kotlin
- Web framework: vertx
- DB: MongoDB
- File storage: Local file storage and AWS s3
- React with typescript with vite
- UI: Shadcn + Tailwind
- Drag and drop: Tailwind + useRef + onDrag events
- auth framework: auth0: If it doesn't work, fallback to access/refresh token mechanism with google auth login.

### Secondary Requirements/Features
- OAuth google login, github login, login with email
- sort by created data, modified date
- drag and drop files onto a highlighted area (frontend-only)
- search your files
- load low resolution preview
- delete feature
- upload folders
- create folders and organise content
- duplicate file deteaction by hasing the name and the contents of the file
- A progress bar for the storage used till now
- Dark mode/Light Mode
- encrypt the files and make the user aware
- suggested for you field with preview
- upload multiple folders at once
- shareble log
- pagination for listing all files
- add caching for faster loading

### Action Plan
- [x] Create architecture diagram on excalidraw
- [x] Finalise all frameworks and technology (backend language, framework, front end ui library, blob storage, metdata DB, docker)
- [X] Design the home page (blindly copy drop box and make improvements)
- [X] Design the signup and login page
- [x] Initial docker setup for backend
- [x] Setup unit testing
- [X] /login & /signup API
- [ ] Initial docker setup for front end
- [ ] user login/signup page
- [ ] user home page
- [ ] /upload API
- [ ] /list API
- [ ] /download API
- [ ] upload button
- [ ] list files
- [ ] download file
- [ ] upload area
- [ ] preview file button (click the file)


### Hard Problems to be aware of
- how to preview the file (front end)
- how to upload the contents of a large file to the server (frontend and backend)
- which blob storage to choose (for deployment purpose
- how to download. What header content type and values should be passed while returning the file?

### Things to take care
- ⁠action plan
- choose one Hue, different saturations for buttons.
- ⁠technologies finalise with reasoning
- ⁠⁠architecture diagram
- ⁠⁠unit testing approach
- ⁠⁠deploying on docker
- ⁠⁠deploying on domain on render



