---
title: "WorksheetDesign"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Abgeleitet von WebWorksheet."
type: docs
url: /de/java/com.aspose.gridweb/worksheetdesign/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control), [com.aspose.gridweb.WebWorksheet](../../com.aspose.gridweb/webworksheet)
```
public class WorksheetDesign extends WebWorksheet
```

Abgeleitet von WebWorksheet. Nur zur Entwurfszeit verwendet.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [WorksheetDesign()](#WorksheetDesign--) | Standardkonstruktor. |
| [WorksheetDesign(MainWeb mw, GridWorksheet gwk)](#WorksheetDesign-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-) | Der Konstruktor mit MainWeb und GridWorksheet |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Passt die Spaltenbreite automatisch an. |
| [autoFitColumn(int columnIndex, int startRow, int endRow)](#autoFitColumn-int-int-int-) | Passt die Spaltenbreite automatisch an. |
| [cancelNewBindRow()](#cancelNewBindRow--) | Bricht die neu hinzugefügte bind row ab und löscht sie. |
| [commitNewBindRow()](#commitNewBindRow--) | Bestätigt die neu hinzugefügte bind row und fügt sie der DataSource hinzu. |
| [copy(WebWorksheet source)](#copy-com.aspose.gridweb.WebWorksheet-) | Kopiert von einem anderen Arbeitsblatt-Objekt. |
| [createAutoGenratedColumns()](#createAutoGenratedColumns--) | Nachdem eine DataSource für das Arbeitsblatt festgelegt wurde, rufen Sie diese Methode auf, um die Bind-Spalten automatisch zu erzeugen. |
| [createNewBindRow()](#createNewBindRow--) | Erstellt eine neue bind row und bindet sie an die DataSource. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Erstellt Zwischensumme im Blatt. |
| [dataBind()](#dataBind--) | Binden Sie das Blatt an die DataSource. |
| [deleteBindRow(int rowNum)](#deleteBindRow-int-) | Löscht eine bind row. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Friert Bereiche an der angegebenen Zelle im Arbeitsblatt ein. |
| [getBindStartColumn()](#getBindStartColumn--) | Im Datenbindungsmodus geben BindStartRow und BindStartColumn die Position des Rasters an, das an die DataSource gebunden werden soll. |
| [getBindStartRow()](#getBindStartRow--) | Im Datenbindungsmodus geben BindStartRow und BindStartColumn die Position des Rasters an, das an die DataSource gebunden werden soll. |
| [getBindingSource()](#getBindingSource--) | Das tatsächlich zur Laufzeit bindende DataSource-Objekt. |
| [getClass()](#getClass--) |  |
| [getCurrentBindRows()](#getCurrentBindRows--) | Ermittelt die Anzahl der Bind-Zeilen im Datenbindungsmodus. |
| [getDataMember()](#getDataMember--) | Ermittelt das DataMember aus der mehrgliedrigen DataSource. |
| [getDataSource()](#getDataSource--) | Ermittelt die DataSource. |
| [getEnableCreateBindColumnHeader()](#getEnableCreateBindColumnHeader--) | Im Datenbindungsmodus gibt an, ob Spaltenkopfzeilen für Bind-Spalten im Blatt erstellt werden sollen. |
| [getIndex()](#getIndex--) | Ermittelt den Index des Objekts innerhalb der Arbeitsblätter. |
| [getName()](#getName--) | Ermittelt den Namen des Blatts. |
| [getUniqueID()](#getUniqueID--) | Ruft die UniqueID im Steuerelement ab. |
| [getValidations()](#getValidations--) | Ruft die Datengültigkeits‑Einstellungs‑Sammlung im Arbeitsblatt ab. |
| [getVisible()](#getVisible--) | Gibt an, ob der Name dieses Blatts in den Blattregisterkarten des Steuerelements angezeigt wird. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Gruppiert Zeilen. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Gruppiert Zeilen. |
| [hashCode()](#hashCode--) |  |
| [isProtected()](#isProtected--) | Ermittelt, ob das Arbeitsblatt geschützt ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllCellsEditable()](#setAllCellsEditable--) | Macht alle Zellen editierbar. Dies ist ein erweitertes Attribut. |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Macht alle Zellen schreibgeschützt. Dies ist ein erweitertes Attribut; beachten Sie, dass dieses Attribut nicht in der tatsächlichen Zelle erhalten bleibt. Wenn Sie den Schutz beibehalten möchten, verwenden Sie bitte setProtect. |
| [setBindStartColumn(int value)](#setBindStartColumn-int-) | Im Datenbindungsmodus geben BindStartRow und BindStartColumn die Position des Rasters an, das an die DataSource gebunden werden soll. |
| [setBindStartRow(int value)](#setBindStartRow-int-) | Im Datenbindungsmodus geben BindStartRow und BindStartColumn die Position des Rasters an, das an die DataSource gebunden werden soll. |
| [setCurrentBindRows(int value)](#setCurrentBindRows-int-) | Ermittelt die Anzahl der Bind-Zeilen im Datenbindungsmodus. |
| [setDataMember(String value)](#setDataMember-java.lang.String-) | Setzt das DataMember aus der mehrgliedrigen DataSource. |
| [setDataSource(Object value)](#setDataSource-java.lang.Object-) | Setzt die DataSource. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Macht einen Zellbereich editierbar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Machen Sie alle Zellen schreibgeschützt, indem Sie die Methode SetAllCellsReadonly aufrufen. |
| [setEnableCreateBindColumnHeader(boolean value)](#setEnableCreateBindColumnHeader-boolean-) | Im Datenbindungsmodus gibt an, ob Spaltenkopfzeilen für Bind-Spalten im Blatt erstellt werden sollen. |
| [setName(String value)](#setName-java.lang.String-) | Setzt den Namen des Blatts. |
| [setProtected(boolean value)](#setProtected-boolean-) | Legt fest, ob das Arbeitsblatt geschützt ist. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Macht einen Zellbereich schreibgeschützt. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Zuerst alle Zellen editierbar machen, indem Sie die Methode SetAllCellsEditable aufrufen. |
| [setVisible(boolean value)](#setVisible-boolean-) | Gibt an, ob der Name dieses Blatts in den Blattregisterkarten des Steuerelements angezeigt wird. |
| [toString()](#toString--) |  |
| [unfreezePanes()](#unfreezePanes--) | Löst das Einfrieren von Bereichen im Arbeitsblatt. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Hebt die Gruppierung von Zeilen auf. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorksheetDesign() {#WorksheetDesign--}
```
public WorksheetDesign()
```


Standardkonstruktor.

### WorksheetDesign(MainWeb mw, GridWorksheet gwk) {#WorksheetDesign-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-}
```
public WorksheetDesign(MainWeb mw, GridWorksheet gwk)
```


Der Konstruktor mit MainWeb und GridWorksheet

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| mw | [MainWeb](../../com.aspose.gridweb/mainweb) |  |
| gwk | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) |  |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Passt die Spaltenbreite automatisch an.

**Remarks**

AutoFitColumn ist eine ungenaue Funktion.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex. |

### autoFitColumn(int columnIndex, int startRow, int endRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int startRow, int endRow)
```


Passt die Spaltenbreite automatisch an. Diese Methode passt eine Spalte basierend auf dem Inhalt eines Zellbereichs innerhalb der Spalte von startRow bis endRow automatisch an. AutoFitColumn ist eine ungenaue Funktion.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | int | Spaltenindex, nullbasiert |
| startRow | int | Startzeilenindex, nullbasiert |
| endRow | int | Endzeilenindex, nullbasiert |

### cancelNewBindRow() {#cancelNewBindRow--}
```
public int cancelNewBindRow()
```


Bricht die neu hinzugefügte bind row ab und löscht sie.

**Returns:**
int – Der Zeilenindex. Wenn keine neu erstellte bind row vorhanden ist, wird -1 zurückgegeben.
### commitNewBindRow() {#commitNewBindRow--}
```
public int commitNewBindRow()
```


Bestätigt die neu hinzugefügte bind row und fügt sie der DataSource hinzu.

**Returns:**
int - Der Zeilenindex der neuen Zeile. Wenn keine Zeile erstellt wird, wird -1 zurückgegeben.
### copy(WebWorksheet source) {#copy-com.aspose.gridweb.WebWorksheet-}
```
public void copy(WebWorksheet source)
```


Kopiert von einem anderen Arbeitsblatt-Objekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [WebWorksheet](../../com.aspose.gridweb/webworksheet) | Das andere Blatt. |

### createAutoGenratedColumns() {#createAutoGenratedColumns--}
```
public void createAutoGenratedColumns()
```


Nachdem eine DataSource für das Arbeitsblatt festgelegt wurde, rufen Sie diese Methode auf, um die Bind-Spalten automatisch zu erzeugen.

### createNewBindRow() {#createNewBindRow--}
```
public int createNewBindRow()
```


Erstellt eine neue bind row und bindet sie an die DataSource.

**Returns:**
int - Der Zeilenindex der neuen Zeile. Wenn keine Zeile erstellt wird, wird -1 zurückgegeben.
### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


Erstellt Zwischensumme im Blatt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnNameRowIndex | int | Der Zeilenindex der Spaltennamenzeile. |
| dataRows | int | Die Anzahl der Datenzeilen. |
| groupByColumnIndex | int | Der Spaltenindex der zu gruppierenden Spalte. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Der Typ der Zwischensumme-Funktion. |
| subtotalColumnIndexList | int[] | Die Spaltenindizes, die zusammengefasst werden sollen. |
| functionLabel | java.lang.String | Die Bezeichnung der Zwischensumme-Funktion. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Der Stil der Gesamtsummenzeile. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Der Stil der Zwischensummenzeile. |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype). Der Zahlentyp der Zwischensummen-Ergebniszellen. |
| customString | java.lang.String | Der benutzerdefinierte Formatstring der Zwischensummen-Ergebniszellen. Kann null sein. |

### dataBind() {#dataBind--}
```
public void dataBind()
```


Binden Sie das Blatt an die DataSource.

### deleteBindRow(int rowNum) {#deleteBindRow-int-}
```
public int deleteBindRow(int rowNum)
```


Löscht eine bind row.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| rowNum | int | Der Zeilenindex. |

**Returns:**
int - Der gelöschte Zeilenindex. Wenn keine Bindungszeile gelöscht wird, wird -1 zurückgegeben.
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
### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Friert Bereiche an der angegebenen Zelle im Arbeitsblatt ein.

**Remarks**

Zeilenindex und Spaltenindex können nicht beide Null sein. Die Anzahl der Zeilen und die Anzahl der Spalten können ebenfalls nicht beide Null sein.

Die ersten beiden Parameter geben die eingefrorene Position an und die letzten beiden Parameter geben den eingefrorenen Bereich im linken oberen Bereich an.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Zeile | int | Zeilenindex. |
| Spalte | int | Spaltenindex. |
| freezedRows | int | Anzahl der sichtbaren Zeilen im oberen Bereich, nicht mehr als Zeilenindex. |
| freezedColumns | int | Anzahl der sichtbaren Spalten im linken Bereich, nicht mehr als Spaltenindex. |

### getBindStartColumn() {#getBindStartColumn--}
```
public int getBindStartColumn()
```


Im Datenbindungsmodus geben BindStartRow und BindStartColumn die Position des Rasters an, das an die DataSource gebunden werden soll.

**Returns:**
int
### getBindStartRow() {#getBindStartRow--}
```
public int getBindStartRow()
```


Im Datenbindungsmodus geben BindStartRow und BindStartColumn die Position des Rasters an, das an die DataSource gebunden werden soll.

**Returns:**
int
### getBindingSource() {#getBindingSource--}
```
public Iterable getBindingSource()
```


Das tatsächlich zur Laufzeit bindende Datenquellenobjekt. Es ist ein DataView-Objekt, wenn die DataSource‑Eigenschaft ein DataSet-, DataTable- oder DataView-Objekt ist.

**Returns:**
java.lang.Iterable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentBindRows() {#getCurrentBindRows--}
```
public int getCurrentBindRows()
```


Ermittelt die Anzahl der Bind-Zeilen im Datenbindungsmodus.

**Returns:**
int
### getDataMember() {#getDataMember--}
```
public String getDataMember()
```


Liest das DataMember aus der mehrgliedrigen DataSource aus. Im Allgemeinen stellt es ein DataTable-Objekt eines DataSet dar.

**Returns:**
java.lang.String
### getDataSource() {#getDataSource--}
```
public Object getDataSource()
```


Liest die DataSource aus. Im Allgemeinen ist es ein DataSet-Objekt.

**Returns:**
java.lang.Object
### getEnableCreateBindColumnHeader() {#getEnableCreateBindColumnHeader--}
```
public boolean getEnableCreateBindColumnHeader()
```


Im Datenbindungsmodus gibt an, ob Spaltenkopfzeilen für Bind-Spalten im Blatt erstellt werden sollen.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


Ermittelt den Index des Objekts innerhalb der Arbeitsblätter.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Ermittelt den Namen des Blatts.

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Ruft die UniqueID im Steuerelement ab.

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


Ruft die Datengültigkeits‑Einstellungs‑Sammlung im Arbeitsblatt ab.

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Gibt an, ob der Name dieses Blatts in den Blattregisterkarten des Steuerelements angezeigt wird.

**Returns:**
boolean
### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Gruppiert Zeilen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | int | Der erste Zeilenindex, der gruppiert werden soll. |
| lastIndex | int | Der letzte Zeilenindex, der gruppiert werden soll. |

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Gruppiert Zeilen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | int | Der erste Zeilenindex, der gruppiert werden soll. |
| lastIndex | int | Der letzte Zeilenindex, der gruppiert werden soll. |
| isHidden | boolean | Gibt an, ob die gruppierten Zeilen ausgeblendet sind. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Liest, ob das Arbeitsblatt geschützt ist. Wenn ein Arbeitsblatt geschützt ist, können alle Zellen nicht bearbeitet werden, außer der Zelle, deren IsLocked‑Eigenschaft false ist.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```


Macht alle Zellen editierbar. Dies ist ein erweitertes Attribut.

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


Macht alle Zellen schreibgeschützt. Dies ist ein erweitertes Attribut; beachten Sie, dass dieses Attribut nicht in der tatsächlichen Zelle erhalten bleibt. Wenn Sie den Schutz beibehalten möchten, verwenden Sie bitte setProtect.

### setBindStartColumn(int value) {#setBindStartColumn-int-}
```
public void setBindStartColumn(int value)
```


Im Datenbindungsmodus geben BindStartRow und BindStartColumn die Position des Rasters an, das an die DataSource gebunden werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBindStartRow(int value) {#setBindStartRow-int-}
```
public void setBindStartRow(int value)
```


Im Datenbindungsmodus geben BindStartRow und BindStartColumn die Position des Rasters an, das an die DataSource gebunden werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setCurrentBindRows(int value) {#setCurrentBindRows-int-}
```
public void setCurrentBindRows(int value)
```


Ermittelt die Anzahl der Bind-Zeilen im Datenbindungsmodus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setDataMember(String value) {#setDataMember-java.lang.String-}
```
public void setDataMember(String value)
```


Setzt das DataMember aus der mehrgliedrigen DataSource. Im Allgemeinen stellt es ein DataTable-Objekt eines DataSet dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setDataSource(Object value) {#setDataSource-java.lang.Object-}
```
public void setDataSource(Object value)
```


Setzt die DataSource. Im Allgemeinen ist es ein DataSet-Objekt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


Macht einen Zellbereich editierbar. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Macht alle Zellen schreibgeschützt, indem die Methode SetAllCellsReadonly aufgerufen wird. Rufen Sie dann diese Methode auf, um den Bereich der Zellen anzugeben, die editierbar sein sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Die Startzeile des Bereichs. |
| startColumn | int | Die Startspalte des Bereichs. |
| rows | int | Die Anzahl der Zeilen. |
| Spalten | int | Die Anzahl der Spalten. |

### setEnableCreateBindColumnHeader(boolean value) {#setEnableCreateBindColumnHeader-boolean-}
```
public void setEnableCreateBindColumnHeader(boolean value)
```


Im Datenbindungsmodus gibt an, ob Spaltenkopfzeilen für Bind-Spalten im Blatt erstellt werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Setzt den Namen des Blatts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setProtected(boolean value) {#setProtected-boolean-}
```
public void setProtected(boolean value)
```


Setzt, ob das Arbeitsblatt geschützt ist. Wenn ein Arbeitsblatt geschützt ist, können alle Zellen nicht bearbeitet werden, außer der Zelle, deren IsLocked‑Eigenschaft false ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


Macht einen Zellbereich schreibgeschützt. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Zuerst alle Zellen editierbar machen, indem die Methode SetAllCellsEditable aufgerufen wird. Dann diese Methode aufrufen, um den Bereich von Zellen anzugeben, der schreibgeschützt sein soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | int | Die Startzeile des Bereichs. |
| startColumn | int | Die Startspalte des Bereichs. |
| rows | int | Die Anzahl der Zeilen. |
| Spalten | int | Die Anzahl der Spalten. |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Gibt an, ob der Name dieses Blatts in den Blattregisterkarten des Steuerelements angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unfreezePanes() {#unfreezePanes--}
```
public void unfreezePanes()
```


Löst das Einfrieren von Bereichen im Arbeitsblatt.

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Hebt die Gruppierung von Zeilen auf.

**Remarks**

Entfernt nur äußere Gruppeninformationen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| firstIndex | int | Der Index der ersten Zeile, die aufgelöst werden soll. |
| lastIndex | int | Der Index der letzten Zeile, die aufgelöst werden soll. |

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

