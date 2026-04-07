# RAG Backend
 A Junior ML Engineer Technical Test.

## Setup
1. Create a virtual environment: `python -m venv venv`
2. Activate it: `.\venv\Scripts\activate` (Windows)
3. Install dependencies: `pip install -r requirements.txt`

## Running the Server
Start the Flask server on port 8000:
`python server.py`
docker run:
`-p 8000:8000 translation-rag-app`
## Testing
Run the provided client script to verify the API:
`python client.py`



# Junior ML Engineer Technical Test

The application is designed to handle translation pair storage, dynamic prompt generation for translation tasks, and a specialized detection system for stammering in text.



### Prerequisites
- Python 3.9 or higher
- `pip` (Python package installer)

### Local Setup
1. **Clone the repository:**
 
   `git clone`

### Install Dependencies:
`pip install -r requirements.txt`

### Run the Server;
`python server.py`

### Run the Test Client:
In a new terminal window, run:
`python client.py`

### Docker Instructions 
To run the application using Docker, follow these steps:

Build the Docker Image:
`docker build -t ml-test-app` 

Run the Container:
`docker run -p 8000:8000 ml-test-app`

The API will be available at http://localhost:8000


   # 📊 Captured Test Results
The following outputs were captured by running the client.py script:
### 1. Populate Database
Line 1: Added translation pair.
...
Line 20: Added translation pair.
(All 20 translation pairs successfully processed)

### 2. Request Prompts
Line 1: Received Translation Prompt.
Translate from en to it.
Query: Good night -> Translation: [Processed]
...
Line 18: Received Translation Prompt.
Translate from it to en.
Query: Ci vediamo -> Translation: [Processed]

### 3. Detect Stammering
Line 1: Response -> No (Expected: No)
Line 3: Response -> Yes (Expected: Yes)
Line 10: Response -> Yes (Expected: Yes)
Line 12: Response -> Yes (Expected: Yes)
(Results captured successfully against expected patterns)
