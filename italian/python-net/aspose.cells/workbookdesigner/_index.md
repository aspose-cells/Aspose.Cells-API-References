---
title: classe WorkbookDesigner
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1600
url: /it/python-net/aspose.cells/workbookdesigner/
is_root: false
---
##  classe WorkbookDesigner
Incapsula l'oggetto che rappresenta un foglio di lavoro di progettazione.



Il tipo WorkbookDesigner espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [WorkbookDesigner()](/cells/it/python-net/aspose.cells/workbookdesigner/__init__/#) | Inizializza una nuova istanza della classe [WorkbookDesigner](/cells/it/python-net/aspose.cells/workbookdesigner).|
| [WorkbookDesigner(workbook)](/cells/it/python-net/aspose.cells/workbookdesigner/__init__/#Workbook) | Inizializza una nuova istanza della classe [WorkbookDesigner](/cells/it/python-net/aspose.cells/workbookdesigner).|


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [workbook](/cells/it/python-net/aspose.cells/workbookdesigner/workbook) | Ottiene e imposta l'oggetto [WorkbookDesigner.workbook](/cells/it/python-net/aspose.cells/workbookdesigner#workbook).|
| [repeat_formulas_with_subtotal](/cells/it/python-net/aspose.cells/workbookdesigner/repeat_formulas_with_subtotal) | Indica se si ripetono le formule con la riga del totale parziale.|
| [update_empty_string_as_null](/cells/it/python-net/aspose.cells/workbookdesigner/update_empty_string_as_null) | Se TRUE, verrà inserito Null se il valore è "";|
| [update_reference](/cells/it/python-net/aspose.cells/workbookdesigner/update_reference) | Indica se i riferimenti in altri fogli di lavoro verranno aggiornati.|
| [calculate_formula](/cells/it/python-net/aspose.cells/workbookdesigner/calculate_formula) | Indica se le formule devono essere calcolate.|
| [call_back](/cells/it/python-net/aspose.cells/workbookdesigner/call_back) | Ottiene e imposta l'interfaccia di callback dell'elaborazione di smartmarker.|
| [line_by_line](/cells/it/python-net/aspose.cells/workbookdesigner/line_by_line) | Indica se elaborare l'indicatore intelligente riga per riga.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [set_data_source(data_source, cells_data_table)](/cells/it/python-net/aspose.cells/workbookdesigner/set_data_source/#str-ICellsDataTable) | Imposta l'origine dati di un oggetto [ICellsDataTable](/cells/it/python-net/aspose.cells/icellsdatatable).|
| [set_data_source(variable, data)](/cells/it/python-net/aspose.cells/workbookdesigner/set_data_source/#str-any) | Imposta l'associazione dati a una variabile.|
| [process()](/cells/it/python-net/aspose.cells/workbookdesigner/process/#) | Elabora gli indicatori intelligenti e popola i valori dell'origine dati.|
| [process(is_preserved)](/cells/it/python-net/aspose.cells/workbookdesigner/process/#bool) | Elabora gli indicatori intelligenti e popola i valori dell'origine dati.|
| [process(sheet_index, is_preserved)](/cells/it/python-net/aspose.cells/workbookdesigner/process/#int-bool) | Elabora gli indicatori intelligenti e popola i valori dell'origine dati.|
| [clear_data_source()](/cells/it/python-net/aspose.cells/workbookdesigner/clear_data_source/#) | Cancella tutte le origini dati.|
| [get_smart_markers()](/cells/it/python-net/aspose.cells/workbookdesigner/get_smart_markers/#) | Restituisce una raccolta di marcatori intelligenti in un foglio di calcolo.|



###  Esempio

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

###  Guarda anche
* modulo [aspose.cells](..)
* classe [ICellsDataTable](/cells/it/python-net/aspose.cells/icellsdatatable)
* classe [WorkbookDesigner](/cells/it/python-net/aspose.cells/workbookdesigner)
