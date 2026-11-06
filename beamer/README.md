# Présentation Beamer — ForestFirePred

Ce dossier contient un template Beamer basé sur les analyses du notebook `ForestFirePred.ipynb`.

## Fichiers
- `ForestFirePred_presentation.tex` : slides (à compléter avec les chiffres du notebook)
- `figures/` : dossier pour mettre les images exportées depuis le notebook (optionnel)

## Compilation (Windows)
1) Installer une distribution LaTeX (MiKTeX ou TeX Live)
2) Compiler :

```bash
pdflatex ForestFirePred_presentation.tex
```

Relancer `pdflatex` une 2e fois si nécessaire.

## Où récupérer les chiffres
- Régression : tableau `reg_summary` dans le notebook (RMSE/MAE + CV 10 folds)
- Classification : tableau `clf_summary` (Accuracy/Precision/Recall/F1 + CV 10 folds)
- Bonus : liste `top4` (Permutation Importance) + tableau de comparaison log vs non-log

## (Option) Ajouter des figures
Si tu veux illustrer :
- histogrammes `area` / `log_area`
- scatter `area vs temp`, `area vs wind`
- matrice de confusion

Je peux aussi te rajouter une cellule dans le notebook pour exporter automatiquement ces figures vers `beamer/figures/`.
