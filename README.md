# mlapp
venv\Scripts\Activate.ps1 
pip install streamlit
pip install matplotlib
pip install -U scikit-learn
streamlit run app.py
docker build -t sal_pred .

docker run -it sal_pred

docker run -it -p 8501:8501 sal_pred