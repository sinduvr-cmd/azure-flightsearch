# Streamlit_Deploy1

Install the dependencies:

```powershell
python -m pip install -r requirements.txt
```

Create `.streamlit/secrets.toml` for local development with the required
`SERP_API_KEY` and `MONGO_URI` values. Never commit this file.

For Streamlit Community Cloud, add both `SERP_API_KEY` and `MONGO_URI` under
**Manage app > Settings > Secrets**. The MongoDB URI should point to the
`flightapp` database.

Run the app locally:

```powershell
streamlit run flight_search_app.py
```
