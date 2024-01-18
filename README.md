# Projet 7 Openclassrooms Data Scientist : Implémentez un modèle de scoring pour octroi de crédit
## Créé par Agnès Regaud
## Sujet :
Vous êtes Data Scientist au sein d'une société financière, nommée "Prêt à dépenser", qui propose des crédits à la consommation pour des personnes ayant peu ou pas du tout d'historique de prêt.
L’entreprise souhaite mettre en œuvre un outil de “scoring crédit” pour calculer la probabilité qu’un client rembourse son crédit, puis classifie la demande en crédit accordé ou refusé. 
Elle souhaite donc développer un algorithme de classification en s’appuyant sur des sources de données variées.
Prêt à dépenser souhaite aussi qu'un dashboard interactif soit développé pour que les chargés de relation client puissent à la fois expliquer de façon la plus transparente possible les décisions d’octroi de crédit, 
mais également permettre à leurs clients de disposer de leurs informations personnelles et de les explorer facilement. 

## Objectifs du projet :
- Traitement du déséquilibre des classes de la target
- Recherche du meilleur modèle ML
- Tracking MLFlow
- Création d’un score métier
- Recherche des meilleurs hyper-paramètres avec GridsearchCV et cross validation
- Interprétabilité locale et globale Shap
- Git/GitHub
- Note méthodologique
- DataDrift evidently
- API flask
- Dashboard dockerisé Streamlit avec prise en compte des utilisateurs en situation de handicap pour les textes et graphiques
- Tests unitaires automatisés avec Pytest
- Déploiement cloud automatisé à partir de GitHub avec Heroku


## Compétences évaluées :
- Définir la stratégie d’élaboration d’un modèle d’apprentissage supervisé
- Évaluer les performances des modèles d’apprentissage supervisé
- Définir et mettre en œuvre un pipeline d’entraînement des modèles
- Déployer un modèle via une API dans le Web
- Définir et mettre en œuvre une stratégie de suivi de la performance d’un modèle
- Réaliser un dashboard pour présenter son travail de modélisation
- Rédiger une note méthodologique afin de communiquer sa démarche de modélisation
- Utiliser un logiciel de version de code pour assurer l’intégration du modèle
- Présenter son travail de modélisation à l'oral

## Ce dossier Github contient donc tous les scripts du projet :
- Dans le dossier API :
    * API.py : fichier python de l'API flask
    * DATA : dossier data 	
        	- Autre : fichier df.csv contient les données client et la réponse de la banque
        - Source : fichier df_predict_ft_reduit.csv contient les données client source réduit selon les features sélectionnées et créées; fichier X_scal.npy contient les données client imputées et scalées

    * MODELS : dossier contenant le modèle de prédiction XGBoost entraîné sur les données d'entraînement
    * tests : dossier de test unitaire avec Pytest
    * Logo.png : logo de la société
    
- Dans le dossier Dashboard :
    * app.py : fichier python du Dashboard streamlit
    * DATA : dossier data 	
        	- Autre : fichier df.csv contient les données client et la réponse de la banque
        - Source : fichier df_predict_ft_reduit.csv contient les données client source réduit selon les features sélectionnées et créées; fichier X_scal.npy contient les données client imputées et scalées

    * MODELS : dossier contenant le modèle de prédiction XGBoost entraîné sur les données d'entraînement
    * Logo.png : logo de la société
    
- Dans le dossier DATA DRIFT evidently :
    * application_train_data_and_target_drift.html : fichier html compte-rendu datadrift
    * file_notarget.html : fichier html compte-rendu data drift, data quality, et data stability
    * score_target_drift.html : analyse Prediction Drift
    
## Liens vers repos Github reliés à Heroku et lien vers l'application hébergée sur Heroku :
- API flask : https://github.com/agnesR23/OC_Projet7_API
- Dashboard streamlit : https://github.com/agnesR23/OC_Projet7_Dashboard
- Application déployée sur Heroku : https://oc-p7-dashboard-ba539a450dd7.herokuapp.com/


