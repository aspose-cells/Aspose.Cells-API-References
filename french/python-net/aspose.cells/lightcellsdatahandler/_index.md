---
title: LightCellsDataHandler classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 990
url: /fr/python-net/aspose.cells/lightcellsdatahandler/
is_root: false
---
##  LightCellsDataHandler classe
Représente le gestionnaire de données de cellules pour la lecture de fichiers de feuille de calcul volumineux en mode léger.



Le type LightCellsDataHandler expose les membres suivants :

###  Méthodes
| Méthode| Description|
| :- | :- |
| [start_sheet(sheet)](/cells/fr/python-net/aspose.cells/lightcellsdatahandler/start_sheet/#Worksheet) | Commence à traiter une feuille de calcul.|
| [start_row(row_index)](/cells/fr/python-net/aspose.cells/lightcellsdatahandler/start_row/#int) | Se prépare à traiter une ligne.|
| [process_row(row)](/cells/fr/python-net/aspose.cells/lightcellsdatahandler/process_row/#Row) | Commence à traiter une ligne.|
| [start_cell(column_index)](/cells/fr/python-net/aspose.cells/lightcellsdatahandler/start_cell/#int) | Se prépare à traiter une cellule.|
| [process_cell(cell)](/cells/fr/python-net/aspose.cells/lightcellsdatahandler/process_cell/#Cell) | Commence à traiter une cellule.|



###  Remarques

Lors de la lecture d'un classeur par ce mode, [LightCellsDataHandler.start_sheet(sheet)](/cells/fr/python-net/aspose.cells/lightcellsdatahandler/start_sheet) sera vérifié lors de la lecture de chaque feuille de calcul dans le classeur.
Pour une feuille, si [LightCellsDataHandler.start_sheet(sheet)](/cells/fr/python-net/aspose.cells/lightcellsdatahandler/start_sheet) donne vrai, alors toutes les données et propriétés des lignes/cellules de cette feuille seront vérifiées
et traitées par l'implémentation de cette interface. Pour chaque ligne, [LightCellsDataHandler.start_row(row_index)](/cells/fr/python-net/aspose.cells/lightcellsdatahandler/start_row) sera appelée pour vérifier si elle doit être traitée.
Si une ligne doit être traitée, les propriétés de cette ligne seront lues en premier et l'utilisateur pourra accéder à ses propriétés par [LightCellsDataHandler.process_row(row)](/cells/fr/python-net/aspose.cells/lightcellsdatahandler/process_row).
si les cellules de la ligne doivent également être traitées, alors [LightCellsDataHandler.process_row(row)](/cells/fr/python-net/aspose.cells/lightcellsdatahandler/process_row) devrait renvoyer vrai, puis [LightCellsDataHandler.start_cell(column_index)](/cells/fr/python-net/aspose.cells/lightcellsdatahandler/start_cell) sera
appelé pour chaque cellule existante dans cette ligne pour vérifier si une cellule doit être traitée. Si une cellule doit être traitée,
alors [LightCellsDataHandler.process_cell(cell)](/cells/fr/python-net/aspose.cells/lightcellsdatahandler/process_cell) sera appelé pour traiter la cellule par la mise en place de cette interface.

###  Voir également
* module [aspose.cells](..)
