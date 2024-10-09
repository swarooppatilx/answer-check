## Technologies Used

- Python 3.12
- Flask
- Flask-MySQLdb
- MySQL
- Bootstrap

### Requirements

- Python 3.12
- MySQL Server

### Install Dependencies

Make sure you have a virtual environment set up. You can create one using:

```bash
python -m venv venv
```

### On Windows

```bash
venv\Scripts\activate
```

### On macOS/Linux
```bash
source venv/bin/activate
```

### Install the required packages:
```bash
pip install -r requirements.txt
```

### Update the config.py file with your MySQL database credentials

```bash
class Config:
    MYSQL_HOST = 'localhost'
    MYSQL_USER = 'your_mysql_user'
    MYSQL_PASSWORD = 'your_mysql_password'
    MYSQL_DB = 'flask_auth'
```

### Create a MySQL database named flask_auth and a users table with the following structure:

```bash
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(255) NOT NULL UNIQUE,
    email VARCHAR(255) NOT NULL UNIQUE,
    password VARCHAR(255) NOT NULL
);
```

### To run the application, execute:

```bash
python app.py
```


