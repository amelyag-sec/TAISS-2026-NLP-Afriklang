# Classification de Commentaires Citoyens - TAISS 2026 / Afriklang

## Description du Projet
Ce projet s'inscrit dans le cadre du test technique TAISS 2026 pour le recrutement d'un stagiaire chez Afriklang. L'objectif est de construire un pipeline PNL (NLP) capable de classifier automatiquement des retours citoyens sur les services publics en 3 catégories : **Satisfaction**, **Insatisfaction**, et **Suggestion**.

## Approche Méthodologique
1. **Prétraitement & Nettoyage** : Conversion en minuscules, suppression de la ponctuation, des chiffres et des stopwords français, tout en préservant le vocabulaire spécifique et les expressions locales en éwé/mina.
2. **Vectorisation** : Utilisation de **TF-IDF** (Term Frequency-Inverse Document Frequency) pour extraire la représentation numérique des textes.
3. **Modélisation & Évaluation** : Comparaison de 4 algorithmes de classification (Régression Logistique, SVM, Naive Bayes et Random Forest) avec une séparation Train/Test (80/20).

## Résultats
- Le modèle de **Régression Logistique** a obtenu la meilleure performance générale avec une **Accuracy de ~83.3%** et un **F1-score Macro de ~0.83**.

## Limites et Améliorations Futures
- **Limites** : Taille restreinte du jeu de données (150 commentaires) et sous-représentation des termes éwé/mina.
- **Pistes d'amélioration** : 
  - Fine-tuning d'un modèle Transformer pré-entraîné multilingue (ex: CamemBERT ou AfriBERTa).
  - Augmentation de données (Data Augmentation) pour enrichir les cas de retours mixtes français/éwé/mina.
