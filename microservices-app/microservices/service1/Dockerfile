FROM python:3.9-slim\nWORKDIR /app\nCOPY . /app\nRUN pip install --no-cache-dir -r requirements.txt\nEXPOSE 5000\nENV NAME World\nCMD ["python", "main.py"]
