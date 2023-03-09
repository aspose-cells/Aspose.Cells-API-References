---
title: region propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 520
url: /fr/python-net/aspose.cells/workbooksettings/region/
is_root: false
---
##  region propriété

Obtient ou définit les paramètres régionaux du classeur.

###  Remarques

1. Paramètres régionaux utilisés par le composant Aspose.Cells pour un classeur chargé à partir du fichier modèle :
je). Pour un fichier XLS, des champs sont définis pour les paramètres régionaux et MS Excel enregistre les données des paramètres régionaux dans le fichier lors de l'enregistrement du fichier XLS.
Nous utilisons donc le region enregistré dans le fichier de modèle du classeur.
Si vous ne souhaitez pas utiliser le region enregistré dans le fichier XLS, veuillez le réinitialiser à celui attendu (par exemple, CountryCode.Default) après avoir chargé le fichier de modèle.
Et, nous enregistrons également la valeur spécifiée par l'utilisateur (par cette méthode) dans le fichier lors de l'enregistrement d'un fichier XLS.
ii). Pour les autres formats de fichier, tels que XLSX, XLSB...etc., aucun champ n'est défini pour les paramètres régionaux dans la spécification du format de fichier.
Nous utilisons donc les paramètres régionaux de l'environnement de l'application pour le classeur.
De plus, la valeur spécifiée par l'utilisateur (par cette méthode) ne peut pas être conservée pour les fichiers générés avec ces formats de fichier.
2. Pour l'effet de vue dans MS Excel :
Les paramètres régionaux appliqués ici ne peuvent prendre effet qu'au moment de l'exécution avec le composant Aspose.Cells et non lors de l'affichage du fichier généré avec MS Excel.
Même pour le fichier XLS généré dans lequel les données de paramètres régionaux spécifiés ont été enregistrées, lors de la visualisation/modification avec MS Excel,
le region utilisé pour effectuer le formatage par MS Excel est toujours les paramètres régionaux par défaut de l'environnement dans lequel MS Excel est exécuté,
pas celui enregistré dans le fichier. C'est le comportement de MS Excel et ne peut pas être modifié par le code.
###  Définition:
```python
@property
def region(self):
    ...
@region.setter
def region(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [CountryCode](/cells/fr/python-net/aspose.cells/countrycode)
* classe [WorkbookSettings](/cells/fr/python-net/aspose.cells/workbooksettings)
