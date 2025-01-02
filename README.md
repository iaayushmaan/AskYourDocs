# AskYourDocs


The is a web application that allows users to upload PDF documents and interact with their content through a question-and-answer system. The application will leverage Natural Language Processing (NLP) to analyze the uploaded documents and provide context-aware answers to the questions asked by users.





##  API documentation

#### Upload PDF Document



```http
  POST /api/v1/upload
```

| Description                |
 | :------------------------- |
 | Allows users to upload PDF documents to the application. The uploaded PDF is stored securely, and its text content is extracted and processed for future queries. |


#### Query PDF Content

```http
  POST /api/v1/query
```
| Description                |
 | :------------------------- |
 | Enables users to ask questions related to the uploaded PDF content. The application processes the query using NLP and returns a context-aware answer.|



## Tools and Technologies:
- Backend: FastAPI
- NLP Processing: LLamaIndex
- Frontend: React.js
## Run Locally

1. Clone the project

```bash
  git clone https://github.com/iaayushmaan/AskYourDocs.git
```

2. Go to the project directory

```bash
  cd ./AskYourDocs
```
### Backend Setup

3. Go to the backend directory
```bash
  cd ./backend
```
4. Create a virtual environment
```bash
  python -m venv env
```
5. Activate the Virtual Environment
```bash
  .\env\Scripts\Activate.ps1
```

6. Install Dependencies
```bash
  pip install -r requirements.txt
```
7. Create a .env file in app and add OPENAI_API_KEY.

8. Run the Application

```bash
  uvicorn app.main:app --reload
```
### Frontend Setup
9. Go to the frontend directory

```bash
  cd ./frontend
```
10. Install Dependencies
```bash
  npm i
```
11. Start the frontend server
```bash
  npm start
```
9. You are live on "http://localhost:3000/".


## Authors

- [@iaayushmaan](https://www.github.com/iaayushmaan)

