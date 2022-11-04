# develop
API Rest para una web de subida y gestión de archivos

1- Clonar el codigo fuente
2- Instalar las dependencias del proyecto: npm install
3- Administracion de la api via postman y ejemplos de RQ por cada recurso:
   localhost:3001/api/1.0/auth/login  (POST)
   {
    "email": "ricardocoelloquezada@gmail.com",
    "password": "1234aa"
    }
   
   localhost:3001/api/1.0/auth/register (POST)
   {
    "email": "ricardocoelloquezada@gmail.com",
    "name": "Roberto Coello",
    "password": "1234aa"
    }
    
    localhost:3001/api/1.0/auth/forgot-password (PUT)
    {
    "email": "ricardocoelloquezada@gmail.com"
    }
    
    localhost:3001/api/1.0/auth/reset-password (PUT)
    {
    "resetLink": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJfaWQiOiI2MzY0NTE2ZWQzMjY4ODlkOTVhNzRiMDAiLCJyb2xlIjoidXNlciIsImlhdCI6MTY2NzUyMjk5NSwiZXhwIjoxNjY3NTI0MTk1fQ.1FxwM3xiFTJBtQjGaEqf1CxUet2V2X_SR9uKOhfDHxc",
    "newPassword": "abc123"
    }
    
    localhost:3001/api/1.0/fileS3/delete/FILE_NAME.EXTENTION (DELETE)
    EXAMPLE: localhost:3001/api/1.0/fileS3/delete/DevianArt.jpeg
    
    localhost:3001/api/1.0/fileS3/download/FILE_NAME.EXTENTION  (GET)
    
    localhost:3001/api/1.0/fileS3/list GET
    
    localhost:3001/api/1.0/fileS3/upload POST
     BODY-> FORM-DATA-> KEY -> FILE -> SELECCIONAR ARCHIVO 
     
     localhost:3001/api/1.0/fileS3//upload-external-img (POTS)
     {
    "urlImage": "https://images.unsplash.com/photo-1605643556877-eb7851356c52?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&ixid=MnwzNzc3MzV8MHwxfHNlYXJjaHw3NHx8aG9sYSUyMGNvbW8lMjBlc3RhcyUyMHF1ZSUyMHRhbHxlbnwwfHx8fDE2Njc1Njk1NzQ&ixlib=rb-4.0.3&q=80&w=400"
      }
      
      localhost:3001/api/1.0/search/photos (POST)
      {
      "search": "hola como estas que tal",
      "page": 4
      }
      
   Nota, existe una constribucion de un programador que revise para guiarme en cuanto a unas validaciones, nose como retirar esa constribucion a pesar 
   de que no estoy utilizando directamente codigo fuente de esta persona.
   
   Muchas gracias
    
