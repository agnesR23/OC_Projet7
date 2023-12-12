# Projet 7 Openclassrooms Datascientist - Repository dashboard -

Ce projet a pour but de déployer un modèle via une API (ici Flask) dans le Web via Heroku en utilisant un dashboard (Streamlit) pour présenter le travail de modélisation. Il comporte aussi un test unitaire à l'aide de Pytest.
Le code source de l'API contient entre autres un calculateur de score pour une demande de crédit bancaire qui retourne au Dashboard la probabilité que le client puisse le rembourser, et qui indique donc si le crédit est accordé ou non. 
Cette partie est le Dashboard qui a été dockerisé puis build and deploy on Heroku.

    
### Dépendances du projet :
```
pip install -r requirements.txt
```

### Découpage des dossiers :
app.py : fichier python du Dashboard streamlit
DATA : dossier data 	
	- Autre : fichier df.csv contient les données client et la réponse de la banque
    - Source : fichier df_predict_ft_reduit.csv contient les données client source réduit selon les features sélectionnées et créées; fichier X_scal.npy contient les données client imputées et scalées

MODELS : dossier contenant le modèle de prédiction XGBoost entraîné sur les données d'entraînement
Logo.png : logo de la société





