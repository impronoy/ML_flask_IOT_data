
# Prerequisites  
1.  Create a MongoDB Atlas cluster.
2.  Create a database called sensors_db with a collection sensors  
  
# Steps on how to run  
1.  Clone the repository using the below command  
git clone url.git
```
2. Open the project in Visual Studio Code and then open a new terminal.  Create a virtual environment using the below command
```
# Windows
py -m venv .venv
# Linux
python -m venv .venv
```
4. Activate the virtual environment
```
# Windows
.\.venv\Scripts\activate
# Linux
source .venv\bin\activate
```
5. Install the dependencies
```
pip install -r requirements.txt
```  
6. Rename the .env.local to .env
```
mv .env.local .env
```  
7. Replace the value of the .env file to your MongoDB Atlas  
```
MONGO_DB_CONN_STRING=mongodb+srv://<DB_USER_NAME>:<DB_PASSWORD>@<MONGO_DB_ATLAS_ENDPOINT>/sensors_db
```
8. Run the Flask server
```
flask run
```
9. Open your browser and type the following URL
```
http://<IP>:5000
```
