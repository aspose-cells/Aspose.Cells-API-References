---
title: LightCellsDataProvider classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1000
url: /fr/python-net/aspose.cells/lightcellsdataprovider/
is_root: false
---
##  LightCellsDataProvider classe
Représente le fournisseur de données pour l'enregistrement de fichiers de feuille de calcul volumineux en mode léger.



Le type LightCellsDataProvider expose les membres suivants :

###  Méthodes
| Méthode| Description|
| :- | :- |
| [start_sheet(sheet_index)](/cells/fr/python-net/aspose.cells/lightcellsdataprovider/start_sheet/#int) | Démarre l'enregistrement d'une feuille de calcul.|
| [next_row()](/cells/fr/python-net/aspose.cells/lightcellsdataprovider/next_row/#) | Obtient la ligne suivante à enregistrer.|
| [start_row(row)](/cells/fr/python-net/aspose.cells/lightcellsdataprovider/start_row/#Row) | Commence à enregistrer les données d'une ligne.|
| [next_cell()](/cells/fr/python-net/aspose.cells/lightcellsdataprovider/next_cell/#) | Obtient la cellule suivante à enregistrer.|
| [start_cell(cell)](/cells/fr/python-net/aspose.cells/lightcellsdataprovider/start_cell/#Cell) | Commence à enregistrer les données d'une cellule.|
| [is_gather_string()](/cells/fr/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/#) |Vérifie si la valeur de chaîne actuelle de la cellule doit être rassemblée dans un pool global.|



###  Remarques

Lors de l'enregistrement d'un classeur par ce mode, [LightCellsDataProvider.start_sheet(sheet_index)](/cells/fr/python-net/aspose.cells/lightcellsdataprovider/start_sheet) sera vérifié lors de l'enregistrement de chaque feuille de calcul dans le classeur.
Pour une feuille, si [LightCellsDataProvider.start_sheet(sheet_index)](/cells/fr/python-net/aspose.cells/lightcellsdataprovider/start_sheet) donne vrai, toutes les données et propriétés des lignes/cellules de cette feuille doivent être enregistrées
seront fournis par l'implémentation de cette interface. En premier lieu, [LightCellsDataProvider.next_row()](/cells/fr/python-net/aspose.cells/lightcellsdataprovider/next_row) sera appelé pour obtenir l'index de ligne suivant à enregistrer.
Si un index de ligne valide est renvoyé (l'index de ligne doit être dans l'ordre croissant pour que les lignes soient enregistrées),
alors un objet Row représentant cette ligne sera fourni pour l'implémentation afin de définir ses propriétés par [LightCellsDataProvider.start_row(row)](/cells/fr/python-net/aspose.cells/lightcellsdataprovider/start_row).
Pour une ligne, [LightCellsDataProvider.next_cell()](/cells/fr/python-net/aspose.cells/lightcellsdataprovider/next_cell) sera vérifié en premier. Si un index de colonne valide est renvoyé (l'index de colonne doit être dans l'ordre croissant pour que toutes les cellules d'une ligne soient enregistrées),
alors un objet Cell représentant cette cellule sera fourni pour implémentation afin de définir ses données et propriétés par [LightCellsDataProvider.start_cell(cell)](/cells/fr/python-net/aspose.cells/lightcellsdataprovider/start_cell).
Une fois les données de cette cellule définies, cette cellule sera enregistrée directement dans le fichier de feuille de calcul généré et la cellule suivante sera vérifiée et traitée.

###  Voir également
* module [aspose.cells](..)
