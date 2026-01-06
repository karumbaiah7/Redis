##### Step 1: Install Prerequisites:

**python --version**

**python3 --version**





##### Step 2: Download/Clone the Repository

Clone using Git (Recommended):





Then navigate into the folder:

**cd memory-box**





##### Step 3: Create a Virtual Environment (optional but recommended)

**python -m venv venv**



Activate the environment:

Windows:

**venv\\Scripts\\activate**



##### Step 4:Navigate Into Backend Folder

**cd backend**



Check files:

**dir**

then run:

**pip install -r requirements.txt**



##### Step 5:Then run the backend:

**python app.py**





##### Step 6— Setup Frontend (If Needed) \[NEW TERMINAL]

Go back to project root:

**cd frontend**



Check content:

**dir**



If you see:

package.json



Then install frontend dependencies:

**npm install**



##### Step 7:run the proper dev server(in frontend folder terminal)

**npm run dev**



After running npm run dev, you’ll see something like:

  VITE vX.X.X  ready in XXX ms



  **Local:   http://localhost:5173/**

  Network: http://192.168.X.X:5173/

Open that Local URL (likely http://localhost:5173) in the browser



*Keep your backend running like before.*



**http://localhost:5173(run in browser)**





{

cd backend

pip install flask

python app.py   ← (Leave running)



(open new terminal)

cd memory-box/frontend

npm install

npm run dev

}


keys \*
127.0.0.1:6379> keys \*

1\) "note:1729844958"

127.0.0.1:6379> ttl note:1729844958

59

