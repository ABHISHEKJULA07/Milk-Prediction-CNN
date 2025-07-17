# Instructions

1. Create virtual env in current folder:

   ```powershell
   python -m venv venv
   ```

2. Activate virtual env:

   ```powershell
   .\venv\Scripts\activate
   ```

3. Install `kagglehub` and `ipykernel`:

   ```powershell
   pip install kagglehub ipykernel
   ```

4. Save dependencies into `requirements.txt`:

   ```powershell
   pip freeze | Set-Content requirements.txt
   ```

5. Put `kaggle.json` in folder called `.kaggle`.

6. Follow the code in main.ipynb.
