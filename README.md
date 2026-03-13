🎮 Flappy Bird - IA Génétique
Flappy Bird est une implémentation du célèbre jeu de même nom, améliorée avec un algorithme génétique permettant d'entraîner automatiquement le jeu à se jouer lui-même. Ce projet utilise un réseau de neurones entièrement connecté pour simuler des stratégies évolutives et améliorer les performances au fil des générations.

🧠 Explication
🕹️ Implémentation du Jeu
Ce projet est une implémentation de Flappy Bird avec Pygame. Le but est simple : un oiseau doit traverser une série d'obstacles en volant à travers des espaces entre des tuyaux verticaux. Le joueur contrôle le mouvement vertical en effectuant des sauts qui compensent la gravité.

🏆 Approche et Résolution du Problème
L'objectif principal était de développer une IA capable d'apprendre à jouer seule. Pour cela, un algorithme génétique a été utilisé. Cet algorithme simule un processus de sélection naturelle, en générant, évoluant et sélectionnant différentes générations d'oiseaux virtuels.

🤖 Intelligence Artificielle
Architecture du Réseau de Neurones
Chaque oiseau est contrôlé par un réseau de neurones entièrement connecté qui décide s'il doit sauter en fonction de son état actuel. L’état inclut :

La position par rapport au prochain tuyau
La vitesse verticale de l’oiseau
D’autres variables environnementales
Algorithme Génétique
L’apprentissage se fait à travers plusieurs générations d’oiseaux :

Sélection : Les oiseaux ayant obtenu les meilleurs scores sont sélectionnés pour la reproduction.
Crossover : Les nouveaux réseaux sont créés en combinant les paramètres de deux parents.
Mutation : De légères modifications aléatoires sont appliquées aux paramètres pour introduire de la diversité.
Grâce à ces étapes répétées, l’IA apprend progressivement à mieux naviguer entre les tuyaux, prouvant ainsi l’efficacité des algorithmes génétiques pour ce type de problème d’apprentissage.

🛠️ Installation
Pour configurer l’environnement de développement local :

# Cloner le dépôt
git clone https://github.com/OUCHNE01/Flappy_Bird.git

# Accéder au dossier du projet
cd Flappy-Bird

# Installer les dépendances Python
pip install -r requirements.txt


🚀 Utilisation
Pour lancer le jeu et voir l’algorithme génétique en action :
python main.py

⚙️ Configuration
Paramètres du jeu : Ajustez la vitesse des tuyaux, la gravité et la dynamique des sauts en modifiant les constantes dans utils.py.
Paramètres évolutifs : Modifiez le taux de mutation ou les critères de fitness dans utils.py et training.py.
