# Tampilan Aplikasi 
```
![image](https://github.com/user-attachments/assets/cef49928-f7d4-46e0-a5c8-cc3a94891903)
![image](https://github.com/user-attachments/assets/220be18c-9967-472d-b599-5605fd75b128)

```
# Struktur Folder

```
src
├── exceptions
│   ├── ClientError.js
│   └── InputError.js
├── server
│   ├── handler.js
│   ├── routes.js
│   └── server.js
└── services
    ├── inferenceService.js
    ├── loadModel.js
    └── storeData.js
.env
DockerFile
package.json
credentials.json
README.md

```


# Cara Deploy

```
markdown

- Open Cloud Console
- git clone [This Repository]
- gcloud builds submit --tag gcr.io/[PROJECT ID]/[PROJECT DIRECTORY]
- gcloud run deploy backend-mlgc \
--image gcr.io/[PROJECT ID]/[PROJECT DIRECTORY] \
--set-env-vars APP_ENV=production,APP_PORT=8080,APP_HOST=0.0.0.0,MODEL_URL=[MODEL URL] \
--platform managed \
--region asia-southeast2 \
--allow-unauthenticated
  
```

# Deployed Backend 

