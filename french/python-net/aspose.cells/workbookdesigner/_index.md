---
title: WorkbookDesigner classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1600
url: /fr/python-net/aspose.cells/workbookdesigner/
is_root: false
---
##  WorkbookDesigner classe
Encapsule l'objet qui représente une feuille de calcul de concepteur.



Le type WorkbookDesigner expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [WorkbookDesigner()](/cells/fr/python-net/aspose.cells/workbookdesigner/__init__/#) | Initialise une nouvelle instance de la classe [WorkbookDesigner](/cells/fr/python-net/aspose.cells/workbookdesigner).|
| [WorkbookDesigner(workbook)](/cells/fr/python-net/aspose.cells/workbookdesigner/__init__/#Workbook) | Initialise une nouvelle instance de la classe [WorkbookDesigner](/cells/fr/python-net/aspose.cells/workbookdesigner).|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [workbook](/cells/fr/python-net/aspose.cells/workbookdesigner/workbook) |Obtient et définit l'objet [WorkbookDesigner.workbook](/cells/fr/python-net/aspose.cells/workbookdesigner#workbook).|
| [repeat_formulas_with_subtotal](/cells/fr/python-net/aspose.cells/workbookdesigner/repeat_formulas_with_subtotal) | Indique s'il faut répéter des formules avec des lignes de sous-totaux.|
| [update_empty_string_as_null](/cells/fr/python-net/aspose.cells/workbookdesigner/update_empty_string_as_null) | Si TRUE, Null sera inséré si la valeur est "" ;|
| [update_reference](/cells/fr/python-net/aspose.cells/workbookdesigner/update_reference) |Indique si les références dans d'autres feuilles de calcul seront mises à jour.|
| [calculate_formula](/cells/fr/python-net/aspose.cells/workbookdesigner/calculate_formula) | Indique si les formules doivent être calculées.|
| [call_back](/cells/fr/python-net/aspose.cells/workbookdesigner/call_back) | Obtient et définit l'interface de rappel du traitement smartmarker.|
| [line_by_line](/cells/fr/python-net/aspose.cells/workbookdesigner/line_by_line) | Indique si le traitement du marqueur intelligent ligne par ligne.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [set_data_source(data_source, cells_data_table)](/cells/fr/python-net/aspose.cells/workbookdesigner/set_data_source/#str-ICellsDataTable) | Définit la source de données d'un objet [ICellsDataTable](/cells/fr/python-net/aspose.cells/icellsdatatable).|
| [set_data_source(variable, data)](/cells/fr/python-net/aspose.cells/workbookdesigner/set_data_source/#str-any) | Définit la liaison de données à une variable.|
| [process()](/cells/fr/python-net/aspose.cells/workbookdesigner/process/#) | Traite les marqueurs intelligents et remplit les valeurs de la source de données.|
| [process(is_preserved)](/cells/fr/python-net/aspose.cells/workbookdesigner/process/#bool) | Traite les marqueurs intelligents et remplit les valeurs de la source de données.|
| [process(sheet_index, is_preserved)](/cells/fr/python-net/aspose.cells/workbookdesigner/process/#int-bool) | Traite les marqueurs intelligents et remplit les valeurs de la source de données.|
| [clear_data_source()](/cells/fr/python-net/aspose.cells/workbookdesigner/clear_data_source/#) | Efface toutes les sources de données.|
| [get_smart_markers()](/cells/fr/python-net/aspose.cells/workbookdesigner/get_smart_markers/#) | Renvoie une collection de marqueurs intelligents dans une feuille de calcul.|



###  Exemples

```python
from aspose.cells import Workbook, WorkbookDesigner

# Create WorkbookDesigner object.
wd = WorkbookDesigner()
# Open the template file (which contains smart markers).
wd.workbook = Workbook("SmartMarker_Designer.xls")
# Initialize your data from data source
# DataSet ds = new DataSet();
# ...
# Set the datatable as the data source.
# wd.SetDataSource(dt);
# Process the smart markers to fill the data into the worksheets.
wd.process(True)
# Save the excel file.
wd.workbook.save("outSmartMarker_Designer.xls")

```

###  Voir également
* module [aspose.cells](..)
* classe [ICellsDataTable](/cells/fr/python-net/aspose.cells/icellsdatatable)
* classe [WorkbookDesigner](/cells/fr/python-net/aspose.cells/workbookdesigner)
