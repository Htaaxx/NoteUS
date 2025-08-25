**Before going to details, our deployments on vercel just include front-end and login, logout so people could see our website you can not use any service on these deployments yet.**

# 🗒️ NoteUS
Welcome to NoteUS, a full-stack machine learning application developed by the Win to Win team as part of the Machine Learning course. NoteUS offers powerful features to help users interact with unstructured content:
* 💬 Question answering from:
   * Uploaded documents (PDF, text, etc.)
   * YouTube video URLs
   * Audio files (speech-to-text processing)
* 🧠 Automatic mind map generation to visualize key concepts and relationships
* 📄 Cheat sheet creation for quick summaries and review
* 🧭 Interactive mind map functionality:
   * Ask and receive context-aware questions
   * Highlight key sections
   * Generate flashcards from selected branches

---


## 👨‍💻 Team Members

| **Name**             | **Major**                                            | **University**                 |
|----------------------|------------------------------------------------------|--------------------------------|
| Tuan-Anh Ha          | Information Technology               | University of Science (VNUHCM) |
| Quang-Thang Duong    | Information Technology             | University of Science (VNUHCM) |
| Quoc-Thang Nguyen    | Information Technology             | University of Science (VNUHCM) |
| Hai-Long Pham-Nguyen | Information Technology              | University of Science (VNUHCM) |
| Thanh-Nghia Vo       | Information Technology   | University of Science (VNUHCM) |

---



## Getting Started (Local Development, manually)
### Clone project
```
git clone https://github.com/Htaaxx/NoteUS/
```
### API detail
```
cd api
python -m venv venv
source venv/bin/activate  # or .\venv\Scripts\activate on Windows
pip install -r requirements.txt
python main.py
```
Runs at http://localhost:8000
### Front-end detail
Built using Next.js, the front-end provides a modern UI for interacting with the APIs and backend.
```
cd front-end
npm install
npm run dev
```
Runs at http://localhost:3000
### database detail
```
cd back-end
npm install
node src/server
```
Runs at http://localhost:5000
### Environment Variables
If needed, you can copy the sample environment files:
```
cp api/.env.example api/.env
cp back-end/.env.example back-end/.env.local
cp front-end/.env.example back-end/.env.local
```
## 🚀 Getting Started (Local Development with Docker)
To run the entire application (API, frontend, and database), simply run:
```
docker-compose up
```
Docker Compose will automatically:
	1.	Start the API
	2.	Wait for the API to become ready
	3.	Start the frontend and database once the API is up
No additional setup is needed — just make sure Docker is running on your machine.

