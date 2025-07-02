# 💊 Medicine Finder

Medicine Finder is a web application built using Flask and PostgreSQL that helps users search for medicines and locate nearby pharmacies that stock them. The app supports user registration, login, and an admin dashboard to manage pharmacy records. It features a clean, responsive UI styled with custom CSS and MDB UI Kit.

## Features

- Search for medicines by name and location
- View a list of nearby pharmacies that stock the medicine
- User authentication (signup/login/logout)
- Admin dashboard for managing pharmacy records
- PostgreSQL-backed data storage
- Search history logging
- Responsive and user-friendly UI

## Tech Stack

- Python (Flask)
- PostgreSQL
- SQLAlchemy + Flask-Migrate
- HTML, CSS, MDB UI Kit
- Jinja2 (template rendering)

## Setup Instructions

1. Clone the repository  
   `git clone https://github.com/your-username/medicine-finder.git && cd medicine-finder`

2. Set up a virtual environment  
   `python -m venv env && source env/bin/activate`  
   *(Windows: `env\Scripts\activate`)*

3. Install dependencies  
   `pip install -r requirements.txt`

4. Configure PostgreSQL database in `app.py`  
   `app.config['SQLALCHEMY_DATABASE_URI'] = 'postgresql://username:password@localhost/medicine_finder'`

5. Run database migrations  
flask db init # only once
flask db migrate -m "initial"
flask db upgrade

6. Start the app  
`python app.py`

7. Visit `http://localhost:5000` in your browser

## Project Structure
├── app.py
├── requirements.txt
├── backup.sql
├── /templates
│ ├── index.html
│ ├── login.html
│ ├── signup.html
│ ├── search_results.html
│ └── ...
├── /static
│ ├── styles.css
│ ├── search-results.css
│ └── ...
├── /migrations
│ └── versions/

## Author

**Anas** — [GitHub](https://github.com/skanas90)

## License

This project is licensed under the [MIT License](LICENSE).
