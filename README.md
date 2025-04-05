# Simulation de Navigation pour le Transport avec Algorithme de Dijkstra

## Aperçu du Projet
Ce notebook Jupyter présente une simulation de recherche de chemin optimisée pour l'industrie du transport. Il implémente **l'algorithme de Dijkstra** pour calculer des itinéraires optimaux pour les piétons et véhicules dans un environnement en grille. Le projet met en avant la planification de trajets, la simulation multi-agents et la visualisation - des composants clés pour les systèmes de transport intelligents (STI).

### Fonctionnalités Clés
- 🗺️ **Analyse de Carte CSV**: Lit des configurations d'environnement (routes, trottoirs) depuis des fichiers CSV.
- 📊 **Représentation par Graphe**: Génère des listes d'adjacence pour une navigation efficace.
- 🚶♂️🚗 **Simulation Multi-Agents**: Gère des déplacements distincts pour piétons et voitures.
- 📈 **Visualisation Matplotlib**: Animation en temps réel des trajectoires.
- 🧠 **Focus Algorithmique**: Implémentation de Dijkstra pour les chemins les plus courts.

## Compétences Démontrées
- **Conception d'Algorithmes**: Implémentation d'algorithmes de graphes pour la logistique transport.
- **Programmation Orientée Objet**: Architecture propre avec classes `L_graph`, `Map`, `Agent`.
- **Gestion de Données**: Lecture efficace de données spatiales depuis CSV.
- **Visualisation de Données**: Affichage dynamique des déplacements et états de l'environnement.
- **Connaissances Sectorielles**: Contraintes des réseaux de transport (ex : voies dédiées).

## Installation
1. **Dépendances** :
   ```bash
   pip install matplotlib numpy jupyter
2. **Fichier CSV** : Mettez à jour le chemin dans `lecture_fichier_csv()` vers votre fichier de carte.

## Utilisation
1. **Définir les Agents** :
    ```python
    Bob = Agent("pedestrian", (2,20), (4,0))    # Piéton : départ=(2,20), arrivée=(4,0)
    Ferrari = Agent("car", (26,10), (0,6))      # Voiture : départ=(26,10), arrivée=(0,6)
    ```
2. **Générer les Chemins** :
    ```python
    generate_paths()
    ```
3. **Lancer la Simulation** :
    ```python
    update_agent_position()  # Lance la visualisation animée
    ```

## Structure du Code

|Classe/Fonction	 | Description |
|-------|--------------------------------|
|  `L_graph`	| Implémentation de Dijkstra pour le calcul de chemins optimaux.    |
|  `Map`  |	Analyse les cartes CSV et génère des listes d'adjacence.   |   |
|   `Agent` |	Simule le déplacement avec capacités de recherche de chemin.    |
|    `plotting()`	| Visualise les positions et l'environnement avec Matplotlib.  |

## Résultats

Les agents se déplacent de manière optimale via les routes (jaune) et trottoirs (vert).

## Améliorations Futures
- Implémentation de l'algorithme A* pour l'optimisation.

