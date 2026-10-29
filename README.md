# Pilotage-des-ventes-multi-produits-Dashboard-Power-BI-
Projet personnel d'analyse et de visualisation de données de ventes multi-produits (France), réalisé avec Power BI : de la modélisation du jeu de données aux tableaux de bord interactifs d'aide à la décision.
Objectif du projet

Simuler le rôle d'un·e Data Analyst chargé·e du reporting commercial d'une entreprise vendant plusieurs produits sur le territoire français : construire un modèle de données fiable, suivre les indicateurs clés de performance (CA, coûts, marge, quantités) et comparer la performance réelle aux objectifs commerciaux fixés par produit.

Données
Base : historique des ventes (ville, département, date de vente, produit, coût de production unitaire, prix de vente unitaire, quantité vendue, chiffre d'affaires)
Départements : référentiel géographique France (ville, département, région administrative)
Objectifs_2020 : objectifs de chiffre d'affaires par produit (minimum, maximum, objectif, % d'atteinte)
Modélisation
Relations entre les tables Base, Départements et Objectifs_2020 (modèle en étoile)
Table de calendrier dédiée pour l'intelligence temporelle (évolution mensuelle)
Mesures DAX : CA Total, Coût Total, Revenu Brut Total, Quantité Totale, Prix Moyen, Marge Brute %, % Atteinte Objectif, Évolution CA vs mois précédent
Tableaux de bord

Page 1 — Indicateurs clés

Cartes KPI : CA Total, Coût Total, Revenu Brut Total, Quantité Totale, Prix Moyen
Évolution du CA par mois, et évolution en % par rapport au mois précédent (mise en forme conditionnelle rouge/vert)
CA et quantités vendues par produit
Carte géographique du CA par ville
Répartition du CA par région administrative

Page 2 — Suivi des objectifs

Comparaison CA réel vs objectif par produit (graphique + tableau avec icônes de mise en forme conditionnelle)
Légende explicite des seuils de performance
Principaux enseignements
Tous les produits dépassent leur objectif de CA 2020, entre 157 % (T-shirt) et 263 % (Chaussure) de l'objectif fixé — un signal qui interroge soit sur le dimensionnement initial des objectifs, soit sur une performance commerciale particulièrement forte sur la période.
La Veste est le produit le plus générateur de chiffre d'affaires (plus de 80 000 €, soit environ un tiers du CA total), loin devant les autres catégories.
Le CA mensuel présente une forte variabilité d'un mois à l'autre plutôt qu'une tendance linéaire, ce qui suggère un intérêt à creuser les facteurs saisonniers ou événementiels dans une prochaine itération du projet.
Le chiffre d'affaires est réparti sur l'ensemble du territoire français, avec une présence dans la majorité des régions administratives plutôt qu'une concentration sur un seul bassin commercial.
Outils utilisés
Power BI Desktop : modélisation, DAX, visualisation
Excel : préparation et structuration initiale des données
Power Query : transformation et nettoyage des données
Limites connues

La colonne "Région administrative" reflète le découpage régional antérieur à la réforme de 2016. Ce choix est assumé et documenté plutôt que corrigé silencieusement.
