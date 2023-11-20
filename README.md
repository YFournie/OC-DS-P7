# Implémenter un modèle de scoring

# 1. Pour voir tout le travail sur ce projet
Bonjour ! Ce repository a été créé dans le cadre d'un projet de formation de Data Scientist.
Il est indissociable des deux autres repositories que vous trouverez à ces adresses :
- Pour l'API (avec Flask) : https://github.com/YFournie/OCDS-P7-API
- Pour le Dashboard (avec Streamlit) : https://github.com/YFournie/OCDS-P7-Dashboard

Ce repository traîte :
- Le prétraîtement des données (fusion des tableaux, feature engineering)
- L'entraînement du modèle (Choix du modèle, Choix du score à optimiser, Optimisation des hyperparamètres, Gestion du déséquilibre des classes)
- Le test du Data Drift 

# 2. Présentation des enjeux
Dans ce projet, on travaille pour une banque, qui reçoit des clients et accepte ou non de leur proposer un crédit. 
On cherche à créer un modèle qui prend la décision à notre place. On fait face à plusieurs problèmes :

- On a dans nos données un très fort déséquilibre des classes à prédire.
- Le coût métier entre un faux positif et un faux négatif est très différent, j'ai donc créé un score adapté.

Les données viennent de ce challenge Kaggle : https://www.kaggle.com/c/home-credit-default-risk/data

Si vous prêtez attention à mes scores de ROC AUC, vous verrez qu'ils ne sont pas très bons lorsqu'on compare à Kaggle, ce n'était pas le but premier de ce projet. Si vous souhaitez faire mieux, il faut retravailler essentiellement le feature engineering.

# 3. Faire tourner ce projet
Pour ce qui est des packages nécessaires, ils sont dans le requirements.txt
La seule chose qu'il vous reste à faire, c'est de modifier le "path" au début de chaque notebook par celui qui vous conviendra, en fonction de votre organisation de fichiers.

# 4. Si vous êtes aussi étudiant chez OC...

... Et que vous tombez sur mon travail, je ne vous encourage pas à le copier, en revanche, vous pouvez vous en inspirer.
Pour le prétraitement des données, je me suis largement inspiré de ce Kernel Kaggle : https://www.kaggle.com/code/willkoehrsen/start-here-a-gentle-introduction
Vous pouvez également vous diriger vers celui-ci.
