# TDS-Project-1


LLM Code Deployment

1. Create a virtual environment

   On Windows (PowerShell):

   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```

2. Install dependencies

   ```powershell
   pip install -r requirements.txt
   ```

3. Run the app with uvicorn

   ```powershell
   uvicorn main:app --reload
   ```

Docker

- Build and run the container

```powershell
docker build -t tds-project-1 .
docker run -p 8000:8000 tds-project-1
```

Notes

- The project expects a FastAPI app instance named `app` in `main.py`.
- Update `requirements.txt` as needed.
