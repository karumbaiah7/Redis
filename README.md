## 🧠 MemoryBox — Temporary Notes App



A lightweight full-stack application that lets users create temporary notes with a custom expiry time. Notes automatically disappear after their TTL expires using Redis’ built-in expiration feature.

###### 

###### **📌 Features**



📝 Create notes with categories (Idea, Goal, Note, Vent, etc.)



⏳ Set a Time-To-Live (TTL) — notes auto-delete when expired



🎨 Modern responsive UI built using React + Vite



⚡ Fast performance using an in-memory NoSQL database (Redis)



🚀 Backend REST API built using Flask



💾 No manual deletion — Redis handles expiry automatically



###### **🏗️ Tech Stack**



Layer	Technology

Frontend	React, Vite, JavaScript

Backend	Python, Flask

Database	Redis (Memurai on Windows)

Other Tools	npm, pip, virtual environment





###### **🧪 System Architecture**



┌────────────┐        HTTP Request         ┌──────────────┐

│  Frontend  │ ───────────────────────────▶ │   Flask API  │

│ React/Vite │                              │ (Backend)    │

└────────────┘ ◀─────────────────────────── └───────▲──────┘

&nbsp;                JSON Response                        │

&nbsp;                                                     │

&nbsp;                                               Redis Client

&nbsp;                                                     │

&nbsp;                                                     ▼

&nbsp;                                           ┌──────────────────┐

&nbsp;                                           │ Redis / Memurai  │

&nbsp;                                           │ (TTL storage)    │

&nbsp;                                           └──────────────────┘





###### **🚀 Getting Started**



1️⃣ Clone the Repository

git clone https://github.com/<your-username>/memory-box.git

cd memory-box



2️⃣ Backend Setup (Flask + Redis)

Create \& activate virtual environment

python -m venv venv

venv\\Scripts\\activate   # On Windows



Install dependencies

pip install flask redis



Start Flask server

cd backend

python app.py





Server runs at:



👉 http://127.0.0.1:5000



3️⃣ Redis Setup (Windows using Memurai)



Download \& install Memurai (Redis compatible):

🔗 https://www.memurai.com/downloads



Make sure it is running as a background service.



4️⃣ Frontend Setup (React + Vite)



Open a new terminal:



cd frontend

npm install

npm run dev





Frontend will run at:



👉 http://localhost:5173/



###### **🎯 Usage**



Type a note in the input box



Select a TTL duration



Choose a category



Click Save



Note appears under "Active Notes"



It automatically disappears after expiration



📷 Screenshots



(Add after testing — just drag images into README)



Interface	Preview

Note Editor	(Image Placeholder)

Saved Notes View	(Image Placeholder)





###### **🧠 Why Redis?**



Redis is a NoSQL in-memory key-value store with native TTL expiration support, making it ideal for:



Temporary data



Notifications



Caching



Session storage



SQL databases cannot auto-expire data, making Redis the best fit.

###### 

###### **🛠️ Future Improvements**



🔔 Add notifications before note expiry



👤 User authentication system



☁️ Deploy using Docker or Render/Vercel



📱 Add mobile-first interface



###### **🧑‍🎓 Project Purpose**



This project was developed as part of a NoSQL mini-project requirement to demonstrate:



Use of a NoSQL database



Real-time data storage and expiration



Full-stack design and implementation

