---
title: WorkbookDesigner Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1600
url: /de/python-net/aspose.cells/workbookdesigner/
is_root: false
---
##  WorkbookDesigner Klasse
Kapselt das Objekt, das ein Designer-Arbeitsblatt darstellt.



Der Typ WorkbookDesigner macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [WorkbookDesigner()](/cells/de/python-net/aspose.cells/workbookdesigner/__init__/#) | Initialisiert eine neue Instanz der Klasse [WorkbookDesigner](/cells/de/python-net/aspose.cells/workbookdesigner).|
| [WorkbookDesigner(workbook)](/cells/de/python-net/aspose.cells/workbookdesigner/__init__/#Workbook) | Initialisiert eine neue Instanz der Klasse [WorkbookDesigner](/cells/de/python-net/aspose.cells/workbookdesigner).|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [workbook](/cells/de/python-net/aspose.cells/workbookdesigner/workbook) | Ruft das Objekt [WorkbookDesigner.workbook](/cells/de/python-net/aspose.cells/workbookdesigner#workbook) ab und legt es fest.|
| [repeat_formulas_with_subtotal](/cells/de/python-net/aspose.cells/workbookdesigner/repeat_formulas_with_subtotal) | Gibt an, ob sich Formeln mit Zwischensummenzeile wiederholen.|
| [update_empty_string_as_null](/cells/de/python-net/aspose.cells/workbookdesigner/update_empty_string_as_null) | Wenn TRUE, wird Null eingefügt, wenn der Wert "" ist;|
| [update_reference](/cells/de/python-net/aspose.cells/workbookdesigner/update_reference) | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden.|
| [calculate_formula](/cells/de/python-net/aspose.cells/workbookdesigner/calculate_formula) | Gibt an, ob Formeln berechnet werden sollen.|
| [call_back](/cells/de/python-net/aspose.cells/workbookdesigner/call_back) | Ruft die Callback-Schnittstelle der Smartmarker-Verarbeitung ab und legt sie fest.|
| [line_by_line](/cells/de/python-net/aspose.cells/workbookdesigner/line_by_line) | Gibt an, ob die intelligente Markierung Zeile für Zeile verarbeitet wird.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [set_data_source(data_source, cells_data_table)](/cells/de/python-net/aspose.cells/workbookdesigner/set_data_source/#str-ICellsDataTable) | Legt die Datenquelle eines [ICellsDataTable](/cells/de/python-net/aspose.cells/icellsdatatable)-Objekts fest.|
| [set_data_source(variable, data)](/cells/de/python-net/aspose.cells/workbookdesigner/set_data_source/#str-any) | Legt die Datenbindung an eine Variable fest.|
| [process()](/cells/de/python-net/aspose.cells/workbookdesigner/process/#) | Verarbeitet die intelligenten Markierungen und füllt die Datenquellenwerte aus.|
| [process(is_preserved)](/cells/de/python-net/aspose.cells/workbookdesigner/process/#bool) | Verarbeitet die intelligenten Markierungen und füllt die Datenquellenwerte aus.|
| [process(sheet_index, is_preserved)](/cells/de/python-net/aspose.cells/workbookdesigner/process/#int-bool) | Verarbeitet die intelligenten Markierungen und füllt die Datenquellenwerte aus.|
| [clear_data_source()](/cells/de/python-net/aspose.cells/workbookdesigner/clear_data_source/#) | Löscht alle Datenquellen.|
| [get_smart_markers()](/cells/de/python-net/aspose.cells/workbookdesigner/get_smart_markers/#) | Gibt eine Sammlung intelligenter Markierungen in einer Tabelle zurück.|



###  Beispiel

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

###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [ICellsDataTable](/cells/de/python-net/aspose.cells/icellsdatatable)
* Klasse [WorkbookDesigner](/cells/de/python-net/aspose.cells/workbookdesigner)
