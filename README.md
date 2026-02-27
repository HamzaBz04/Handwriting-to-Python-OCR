# Handwriting-to-Python-OCR
# ✍️ Handwriting to Python OCR : Digitalisation d'Algorithmes Manuscrits

Ce projet est un pipeline complet de Deep Learning et de Computer Vision permettant de transformer une image de pseudo-code algorithmique écrit à la main en un script Python exécutable. 

Projet de fin de module réalisé par : Hamza BOUAZZA

## 🚀 Fonctionnalités (Le Pipeline)
1. **Prétraitement visuel (OpenCV) :** Binarisation d'Otsu pour isoler l'encre et éliminer le bruit du papier.
2. **Inférence IA (TrOCR) :** Utilisation d'un modèle Transformer de Microsoft (`microsoft/trocr-base-handwritten`) fine-tuné sur notre dataset (Modèle V3).
3. **Post-traitement Sémantique (Regex) :** Correction automatique des hallucinations visuelles (flèches d'affectation, formatage des variables).
4. **Transpilation Python :** Traduction des mots-clés algorithmiques et gestion automatique de l'indentation.

## 📊 Performances
* Modèle de base : 55 % de précision.
* **Modèle V3 Optimisé : 70 % de précision (1 - CER).**
* *Note : Les erreurs restantes sont majoritairement corrigées par l'étape de post-traitement Regex.*

## 🔗 Ressources
* **Code source :** Consultez le fichier `pipeline.ipynb` pour voir le code.
* **Présentation :** Le fichier PDF `Handwriting_to_python.pdf` détaille notre démarche scientifique.
* **Dataset & Modèle :** *https://drive.google.com/file/d/1gjPJ1_ypTa9VEQxVcTl-kMLXg7EZWCcn/view?usp=sharing.*
