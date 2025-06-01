---
name: agile final template
about: yhis tempate's for users stories
title: ''
labels: ''
assignees: ''

---

**En tant que** utilisateur
 **J'ai besoin de** pouvoir créer un nouveau produit avec ses détails (nom, description, prix, etc.), 
 **Pour que** les utilisateurs puissent le consulter et l'acheter. 
   
 ### Détails et hypothèses
 * Seuls les utilisateurs avec rôle admin peuvent créer des produits

 * Les champs obligatoires sont : nom, prix, catégorie

 * Le prix doit être positif

 * Un produit créé est immédiatement visible dans le catalogue
   
 ### Critères d'acceptation  
   
 ```gherkin
 Étant donné que je suis connecté en tant qu'administrateur
Quand je remplis le formulaire de création avec des données valides
Alors le produit est enregistré dans le catalogue

Étant donné que je suis connecté en tant qu'administrateur
Quand j'essaie de créer un produit avec un prix négatif
Alors je reçois un message d'erreur et le produit n'est pas créé
 ```
