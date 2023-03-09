---
title: ExportTableOptions classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 550
url: /fr/python-net/aspose.cells/exporttableoptions/
is_root: false
---
##  ExportTableOptions classe
Représente toutes les options de table d'exportation.



Le type ExportTableOptions expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [ExportTableOptions()](/cells/fr/python-net/aspose.cells/exporttableoptions/__init__/#) | Construit une nouvelle instance de ExportTableOptions|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [export_column_name](/cells/fr/python-net/aspose.cells/exporttableoptions/export_column_name) | Indique si les données de la première ligne sont exportées vers le nom de colonne du DataTable.<br/> La valeur par défaut est faux.|
| [skip_error_value](/cells/fr/python-net/aspose.cells/exporttableoptions/skip_error_value) | Indique si la valeur non valide est ignorée pour la colonne.<br/> Par exemple, si le type de colonne est decimal , la valeur est supérieure à decimal.MaxValue<br/>et cette propriété est vraie, nous ne lancerons plus d'exception.<br/> La valeur par défaut est faux.|
| [plot_visible_cells](/cells/fr/python-net/aspose.cells/exporttableoptions/plot_visible_cells) | Exporte uniquement les cellules visibles.|
| [plot_visible_rows](/cells/fr/python-net/aspose.cells/exporttableoptions/plot_visible_rows) | Exporte uniquement les lignes visibles.|
| [plot_visible_columns](/cells/fr/python-net/aspose.cells/exporttableoptions/plot_visible_columns) | Exporte uniquement les colonnes visibles.|
| [export_as_string](/cells/fr/python-net/aspose.cells/exporttableoptions/export_as_string) | Exporte la valeur de chaîne des cellules vers le DataTable.|
| [export_as_html_string](/cells/fr/python-net/aspose.cells/exporttableoptions/export_as_html_string) | Exporte la valeur de chaîne html des cellules vers le DataTable.|
| [format_strategy](/cells/fr/python-net/aspose.cells/exporttableoptions/format_strategy) | Obtient et définit la stratégie de format lors de l'exportation de la valeur en tant que valeur de chaîne.|
| [check_mixed_value_type](/cells/fr/python-net/aspose.cells/exporttableoptions/check_mixed_value_type) |False, Aspose.Cells définira le type de DataColumn par le type de valeur de la première ligne pour les performances.<br/> True, Aspose.Cells vérifiera si le type de valeur dans la colonne est mélangé avant de définir le type de DataColumn<br/> Et le type de valeur est mélangé, le type de DataColumn sera une chaîne.|
| [is_vertical](/cells/fr/python-net/aspose.cells/exporttableoptions/is_vertical) | True si une ligne dans le fichier Workbook représente une ligne dans DataTable. False si une colonne dans le fichier Workbook représente une ligne dans DataTable.|
| [indexes](/cells/fr/python-net/aspose.cells/exporttableoptions/indexes) |Les index des colonnes/lignes qui doivent être exportées.|
| [rename_strategy](/cells/fr/python-net/aspose.cells/exporttableoptions/rename_strategy) | Stratégie pour les noms de colonnes en double.|



###  Voir également
* module [aspose.cells](..)
