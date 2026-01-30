# SDD311-BYOL
## Bootstrap Your Own Latent (BYOL)
**Self-Supervised Representation Learning without Negative Pairs**

---

## Description

Ce dépôt contient un **notebook pédagogique et expérimental** consacré à la méthode **BYOL (Bootstrap Your Own Latent)**, introduite par Grill et al. (NeurIPS 2020).

Le notebook accompagne une présentation orale réalisée dans le cadre du cours **Deep Learning Demo – Évaluation 2025–2026**.  
Il a pour objectif de **rendre observables les mécanismes théoriques décrits dans l’article**, à travers des expériences simples et reproductibles.

L’accent est mis sur :
- l’apprentissage de représentations auto-supervisées
- le rôle des *negative pairs* en contrastive learning
- le phénomène de *representation collapse*
- la manière dont BYOL évite ce collapse sans paires négatives

---

## Référence

> J.-B. Grill, F. Strub, F. Altché, et al.  
> **Bootstrap Your Own Latent: A New Approach to Self-Supervised Learning**  
> NeurIPS 2020

---

## Contenu du notebook

Le notebook suit la progression conceptuelle suivante :

1. Apprentissage de représentations et augmentations de données  
2. Baseline contrastive (InfoNCE)  
3. Collapse sans negative pairs (loss attractive uniquement)  
4. Principe de BYOL  
5. Architecture online / target  
6. Stop-gradient et mise à jour EMA  
7. Entraînement BYOL  
8. Analyse expérimentale :
   - évolution des losses
   - variance des représentations
   - visualisations (PCA)
   - comparaisons entre méthodes

Les expériences sont volontairement limitées en nombre d’epochs afin de rester exécutables sur CPU.

---

## Environnement et exécution recommandée

- **Google Colab (CPU)**  
  Le notebook est conçu pour être exécuté sans GPU.
