---
title: "WorkbookDesigner"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das eine Designer-Tabelle darstellt."
type: docs
url: /de/java/com.aspose.cells/workbookdesigner/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookDesigner
```

Kapselt das Objekt, das eine Designer-Tabelle darstellt.

**Example**

```
         //Create WorkbookDesigner object.
         WorkbookDesigner wd = new WorkbookDesigner();
         //Open the template file (which contains smart markers).
         wd.setWorkbook(new Workbook("SmartMarker_Designer.xls"));
 
         //Initialize your data from data source
         //DataSet ds = new DataSet();
 
 
         //Set the datatable as the data source.
         //wd.SetDataSource(dt);
         //Process the smart markers to fill the data into the worksheets.
         wd.process(true);
         //Save the excel file.
         wd.getWorkbook().save("outSmartMarker_Designer.xls");
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [WorkbookDesigner()](#WorkbookDesigner--) | Initialisiert eine neue Instanz der [WorkbookDesigner](../../com.aspose.cells/workbookdesigner) Klasse. |
| [WorkbookDesigner(Workbook workbook)](#WorkbookDesigner-com.aspose.cells.Workbook-) | Initialisiert eine neue Instanz der [WorkbookDesigner](../../com.aspose.cells/workbookdesigner) Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [clearDataSource()](#clearDataSource--) | Löscht alle Datenquellen. |
| [containsVariables()](#containsVariables--) | Gibt an, ob das erste Arbeitsblatt benutzerdefinierte Variablen enthält. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateFormula()](#getCalculateFormula--) | Gibt an, ob Formeln berechnet werden sollen. |
| [getCallBack()](#getCallBack--) | Ruft die Callback‑Schnittstelle der Verarbeitung von Smartmarker ab. |
| [getClass()](#getClass--) |  |
| [getEnableHeaderFooterMarkers()](#getEnableHeaderFooterMarkers--) | Gibt an, ob Kopf-/Fußzeile Smartmarker enthält und zusammen verarbeitet werden soll. |
| [getLineByLine()](#getLineByLine--) | Gibt an, ob die Verarbeitung des Smartmarkers zeilenweise erfolgt. |
| [getRepeatFormulasWithSubtotal()](#getRepeatFormulasWithSubtotal--) | Gibt an, ob Formeln mit Zwischensummenzeile wiederholt werden. |
| [getSmartMarkers()](#getSmartMarkers--) | Gibt eine Sammlung von Smartmarkern in einer Tabellenkalkulation zurück. |
| [getSortDataSource()](#getSortDataSource--) | Gibt an, ob die Datenquelle sortiert wird. |
| [getUpdateEmptyStringAsNull()](#getUpdateEmptyStringAsNull--) | Wenn TRUE, wird Null eingefügt, wenn der Wert "" ist; |
| [getUpdateReference()](#getUpdateReference--) | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |
| [getVariablesWorksheetName()](#getVariablesWorksheetName--) | Ruft den Namen des Arbeitsblatts ab, das Variablen‑Smartmarker enthält. |
| [getWorkbook()](#getWorkbook--) | Ruft das [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--) Objekt ab. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process()](#process--) | Verarbeitet die Smartmarker und füllt die Werte der Datenquelle. |
| [process(boolean isPreserved)](#process-boolean-) | Verarbeitet die Smartmarker und füllt die Werte der Datenquelle. |
| [process(Range range, boolean isPreserved)](#process-com.aspose.cells.Range-boolean-) | Verarbeitet die Smartmarker und füllt die Werte der Datenquelle. |
| [process(int sheetIndex, boolean isPreserved)](#process-int-boolean-) | Verarbeitet die Smartmarker und füllt die Werte der Datenquelle. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Gibt an, ob Formeln berechnet werden sollen. |
| [setCallBack(ISmartMarkerCallBack value)](#setCallBack-com.aspose.cells.ISmartMarkerCallBack-) | Setzt die Callback‑Schnittstelle der Verarbeitung von Smartmarker. |
| [setContainsVariables(boolean value)](#setContainsVariables-boolean-) | Gibt an, ob das erste Arbeitsblatt benutzerdefinierte Variablen enthält. |
| [setDataSource(String dataSource, ICellsDataTable cellsDataTable)](#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-) | Setzt die Datenquelle eines [ICellsDataTable](../../com.aspose.cells/icellsdatatable) Objekts. |
| [setDataSource(String variable, Object data)](#setDataSource-java.lang.String-java.lang.Object-) | Setzt die Datenbindung zu einer Variablen. |
| [setDataSource(String dataSource, ResultSet rs)](#setDataSource-java.lang.String-java.sql.ResultSet-) | Setzt die Datenquelle. |
| [setDataSource(String dataSource, ResultSet rs, int rowCount)](#setDataSource-java.lang.String-java.sql.ResultSet-int-) | Setzt die Datenquelle. |
| [setDataSource(ResultSet rs)](#setDataSource-java.sql.ResultSet-) | Setzt die Datenquelle. |
| [setEnableHeaderFooterMarkers(boolean value)](#setEnableHeaderFooterMarkers-boolean-) | Gibt an, ob Kopf-/Fußzeile Smartmarker enthält und zusammen verarbeitet werden soll. |
| [setJsonDataSource(String name, String json)](#setJsonDataSource-java.lang.String-java.lang.String-) | Setzt den JSON‑Stringwert als Datenquelle für Smartmarker. |
| [setLineByLine(boolean value)](#setLineByLine-boolean-) | Gibt an, ob die Verarbeitung des Smartmarkers zeilenweise erfolgt. |
| [setRepeatFormulasWithSubtotal(boolean value)](#setRepeatFormulasWithSubtotal-boolean-) | Gibt an, ob Formeln mit Zwischensummenzeile wiederholt werden. |
| [setSortDataSource(boolean value)](#setSortDataSource-boolean-) | Gibt an, ob die Datenquelle sortiert wird. |
| [setUpdateEmptyStringAsNull(boolean value)](#setUpdateEmptyStringAsNull-boolean-) | Wenn TRUE, wird Null eingefügt, wenn der Wert "" ist; |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden. |
| [setVariablesWorksheetName(String value)](#setVariablesWorksheetName-java.lang.String-) | Setzt den Namen des Arbeitsblatts, das Variablen‑Smartmarker enthält. |
| [setWorkbook(Workbook value)](#setWorkbook-com.aspose.cells.Workbook-) | Setzt das [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--) Objekt. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookDesigner() {#WorkbookDesigner--}
```
public WorkbookDesigner()
```


Initialisiert eine neue Instanz der [WorkbookDesigner](../../com.aspose.cells/workbookdesigner) Klasse.

### WorkbookDesigner(Workbook workbook) {#WorkbookDesigner-com.aspose.cells.Workbook-}
```
public WorkbookDesigner(Workbook workbook)
```


Initialisiert eine neue Instanz der [WorkbookDesigner](../../com.aspose.cells/workbookdesigner) Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Die Vorlagen‑Arbeitsbuchdatei. |

### clearDataSource() {#clearDataSource--}
```
public void clearDataSource()
```


Löscht alle Datenquellen.

### containsVariables() {#containsVariables--}
```
public boolean containsVariables()
```


Gibt an, ob das erste Arbeitsblatt benutzerdefinierte Variablen enthält.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft WorkbookDesigner.VariablesWorksheetName. Diese Eigenschaft wird 3 Monate später, seit September 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
boolean
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Gibt an, ob Formeln berechnet werden sollen.

**Returns:**
boolean
### getCallBack() {#getCallBack--}
```
public ISmartMarkerCallBack getCallBack()
```


Ruft die Callback‑Schnittstelle der Verarbeitung von Smartmarker ab.

**Returns:**
[ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableHeaderFooterMarkers() {#getEnableHeaderFooterMarkers--}
```
public boolean getEnableHeaderFooterMarkers()
```


Gibt an, ob Kopf-/Fußzeile Smartmarker enthält und zusammen verarbeitet werden soll.

**Returns:**
boolean
### getLineByLine() {#getLineByLine--}
```
public boolean getLineByLine()
```


Gibt an, ob die Verarbeitung des Smartmarkers zeilenweise erfolgt.

**Remarks**

HINWEIS: Diese Klasse ist jetzt veraltet. Bitte verwenden Sie stattdessen Bereichs‑Smartmarker. Diese Eigenschaft wird 12 Monate später, seit Juli 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Returns:**
boolean
### getRepeatFormulasWithSubtotal() {#getRepeatFormulasWithSubtotal--}
```
public boolean getRepeatFormulasWithSubtotal()
```


Gibt an, ob Formeln mit Zwischensummenzeile wiederholt werden.

**Returns:**
boolean
### getSmartMarkers() {#getSmartMarkers--}
```
public String[] getSmartMarkers()
```


Gibt eine Sammlung von Smartmarkern in einer Tabellenkalkulation zurück.

**Remarks**

Bei jedem Aufruf wird ein String‑Array erstellt. Das Array wird sortiert und duplizierte Werte werden entfernt.

**Returns:**
java.lang.String[] – Eine Sammlung von Smart‑Markern
### getSortDataSource() {#getSortDataSource--}
```
public boolean getSortDataSource()
```


Gibt an, ob die Datenquelle sortiert wird.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Diese Eigenschaft wird 12 Monate später, seit Oktober 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben. Json‑Datenquelle wird sortiert, wenn der Smart‑Marker aufsteigende und absteigende Parameter enthält.

**Returns:**
boolean
### getUpdateEmptyStringAsNull() {#getUpdateEmptyStringAsNull--}
```
public boolean getUpdateEmptyStringAsNull()
```


Wenn TRUE, wird Null eingefügt, wenn der Wert "" ist;

**Returns:**
boolean
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```


Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden.

**Returns:**
boolean
### getVariablesWorksheetName() {#getVariablesWorksheetName--}
```
public String getVariablesWorksheetName()
```


Ruft den Namen des Arbeitsblatts ab, das Variablen‑Smartmarker enthält.

**Returns:**
java.lang.String
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Ruft das [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--) Objekt ab.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### process() {#process--}
```
public void process()
```


Verarbeitet die Smartmarker und füllt die Werte der Datenquelle.

### process(boolean isPreserved) {#process-boolean-}
```
public void process(boolean isPreserved)
```


Verarbeitet die Smartmarker und füllt die Werte der Datenquelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isPreserved | boolean | True, wenn der nicht erkannte Smart‑Marker erhalten bleibt. |

### process(Range range, boolean isPreserved) {#process-com.aspose.cells.Range-boolean-}
```
public void process(Range range, boolean isPreserved)
```


Verarbeitet die Smartmarker und füllt die Werte der Datenquelle.

**Remarks**

HINWEIS: Diese Klasse ist jetzt veraltet. Verwenden Sie stattdessen Range‑Smart‑Marker. Diese Eigenschaft wird 12 Monate später, seit Juli 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | [Range](../../com.aspose.cells/range) | Der zu verarbeitende Bereich |
| isPreserved | boolean | True, wenn der nicht erkannte Smart‑Marker erhalten bleibt. |

### process(int sheetIndex, boolean isPreserved) {#process-int-boolean-}
```
public void process(int sheetIndex, boolean isPreserved)
```


Verarbeitet die Smartmarker und füllt die Werte der Datenquelle.

**Remarks**

Diese Methode arbeitet auf Arbeitsblatt‑Ebene.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sheetIndex | int | Arbeitsblatt‑Index. |
| isPreserved | boolean | True, wenn der nicht erkannte Smart‑Marker erhalten bleibt. |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


Gibt an, ob Formeln berechnet werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCallBack(ISmartMarkerCallBack value) {#setCallBack-com.aspose.cells.ISmartMarkerCallBack-}
```
public void setCallBack(ISmartMarkerCallBack value)
```


Setzt die Callback‑Schnittstelle der Verarbeitung von Smartmarker.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ISmartMarkerCallBack](../../com.aspose.cells/ismartmarkercallback) |  |

### setContainsVariables(boolean value) {#setContainsVariables-boolean-}
```
public void setContainsVariables(boolean value)
```


Gibt an, ob das erste Arbeitsblatt benutzerdefinierte Variablen enthält.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft WorkbookDesigner.VariablesWorksheetName. Diese Eigenschaft wird 3 Monate später, seit September 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setDataSource(String dataSource, ICellsDataTable cellsDataTable) {#setDataSource-java.lang.String-com.aspose.cells.ICellsDataTable-}
```
public void setDataSource(String dataSource, ICellsDataTable cellsDataTable)
```


Setzt die Datenquelle eines [ICellsDataTable](../../com.aspose.cells/icellsdatatable) Objekts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataSource | java.lang.String | Der Name der Datenquelle. |
| cellsDataTable | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | Datentabelle. |

### setDataSource(String variable, Object data) {#setDataSource-java.lang.String-java.lang.Object-}
```
public void setDataSource(String variable, Object data)
```


Setzt die Datenbindung zu einer Variablen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| variable | java.lang.String | Variablenname, erstellt mit Smart‑Marker. |
| Daten | java.lang.Object | Quelldaten. |

### setDataSource(String dataSource, ResultSet rs) {#setDataSource-java.lang.String-java.sql.ResultSet-}
```
public void setDataSource(String dataSource, ResultSet rs)
```


Setzt die Datenquelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataSource | java.lang.String | Der Name der Datenquelle. |
| rs | java.sql.ResultSet | Der Ergebnis‑Datensatz. |

### setDataSource(String dataSource, ResultSet rs, int rowCount) {#setDataSource-java.lang.String-java.sql.ResultSet-int-}
```
public void setDataSource(String dataSource, ResultSet rs, int rowCount)
```


Setzt die Datenquelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dataSource | java.lang.String | Der Name der Datenquelle. |
| rs | java.sql.ResultSet | Der Ergebnis‑Datensatz. |
| rowCount | int | Die Datenanzahl des angegebenen Ergebnis‑Datensatzes. Sie sollte die exakte Zeilenanzahl oder -1 sein; Wenn der Ergebnis‑Datensatz nur vorwärts lesbar ist, muss der Benutzer hier die genaue Zeilenanzahl angeben, andernfalls wird der Smart‑Marker möglicherweise nicht korrekt verarbeitet, wenn das Attribut \"noadd\" des Smart‑Markers nicht gesetzt ist. |

### setDataSource(ResultSet rs) {#setDataSource-java.sql.ResultSet-}
```
public void setDataSource(ResultSet rs)
```


Setzt die Datenquelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rs | java.sql.ResultSet | Der Ergebnis‑Datensatz. |

### setEnableHeaderFooterMarkers(boolean value) {#setEnableHeaderFooterMarkers-boolean-}
```
public void setEnableHeaderFooterMarkers(boolean value)
```


Gibt an, ob Kopf-/Fußzeile Smartmarker enthält und zusammen verarbeitet werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setJsonDataSource(String name, String json) {#setJsonDataSource-java.lang.String-java.lang.String-}
```
public void setJsonDataSource(String name, String json)
```


Setzt den JSON‑Stringwert als Datenquelle für Smartmarker.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String | Der Name der Tabelle. Wenn der Wert von JSON ein Objekt darstellt, kann er null sein. |
| JSON | java.lang.String | Der Wert des JSON‑Strings. |

### setLineByLine(boolean value) {#setLineByLine-boolean-}
```
public void setLineByLine(boolean value)
```


Gibt an, ob die Verarbeitung des Smartmarkers zeilenweise erfolgt.

**Remarks**

HINWEIS: Diese Klasse ist jetzt veraltet. Bitte verwenden Sie stattdessen Bereichs‑Smartmarker. Diese Eigenschaft wird 12 Monate später, seit Juli 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRepeatFormulasWithSubtotal(boolean value) {#setRepeatFormulasWithSubtotal-boolean-}
```
public void setRepeatFormulasWithSubtotal(boolean value)
```


Gibt an, ob Formeln mit Zwischensummenzeile wiederholt werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSortDataSource(boolean value) {#setSortDataSource-boolean-}
```
public void setSortDataSource(boolean value)
```


Gibt an, ob die Datenquelle sortiert wird.

**Remarks**

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Diese Eigenschaft wird 12 Monate später, seit Oktober 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben. Json‑Datenquelle wird sortiert, wenn der Smart‑Marker aufsteigende und absteigende Parameter enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setUpdateEmptyStringAsNull(boolean value) {#setUpdateEmptyStringAsNull-boolean-}
```
public void setUpdateEmptyStringAsNull(boolean value)
```


Wenn TRUE, wird Null eingefügt, wenn der Wert "" ist;

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```


Gibt an, ob Verweise in anderen Arbeitsblättern aktualisiert werden.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setVariablesWorksheetName(String value) {#setVariablesWorksheetName-java.lang.String-}
```
public void setVariablesWorksheetName(String value)
```


Setzt den Namen des Arbeitsblatts, das Variablen‑Smartmarker enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setWorkbook(Workbook value) {#setWorkbook-com.aspose.cells.Workbook-}
```
public void setWorkbook(Workbook value)
```


Setzt das [getWorkbook()](../../com.aspose.cells/workbookdesigner\#getWorkbook--) Objekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Workbook](../../com.aspose.cells/workbook) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

