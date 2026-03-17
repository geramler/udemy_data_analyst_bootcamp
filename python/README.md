# Udemy Data Analyst Bootcamp - Python

This project is configured to run Jupyter notebooks with Python 3.12.

## 1) Push to GitHub (current machine)

```bash
cd /home/gerardo/Git/udemy_data_analyst_bootcamp/python
git branch -M main
git add .
git commit -m "Initial project setup for notebooks"
# Replace with your repository URL
git remote add origin https://github.com/<your-username>/<your-repo>.git
git push -u origin main
```

## 2) Clone and run on another machine

```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
python -m ipykernel install --user --name udemy-notebooks --display-name "Python (udemy notebooks)"
```

Then open VS Code, open the notebook, and select the kernel **Python (udemy notebooks)**.

## 3) Run Jupyter directly (optional)

```bash
source .venv/bin/activate
jupyter lab
```

## Notes
- If `python3 -m venv .venv` fails on Ubuntu/Debian, install venv support:
  ```bash
  sudo apt update && sudo apt install -y python3-venv
  ```
