# Setup Guide

## Windows

```cmd
# Install Python from python.org (check "Add to PATH")
python --version

# Clone and setup
git clone https://github.com/yourusername/project-grading-system.git
cd project-grading-system
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

## macOS/Linux

```bash
# Check Python
python3 --version

# Clone and setup
git clone https://github.com/yourusername/project-grading-system.git
cd project-grading-system
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

## Email Setup (Optional)

Edit `multaka/settings.py`:
```python
EMAIL_HOST_USER = 'your-email@gmail.com'
EMAIL_HOST_PASSWORD = 'your-gmail-app-password'
```

## Troubleshooting

- **Python not found:** Add Python to PATH or use `python3`
- **Module errors:** Run `pip install -r requirements.txt`
- **Port in use:** Use `python manage.py runserver 8080`
