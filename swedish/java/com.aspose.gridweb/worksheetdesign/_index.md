---
title: "WorksheetDesign"
second_title: "Aspose.Cells för Java API-referens"
description: "Ärvd från WebWorksheet."
type: docs
url: /sv/java/com.aspose.gridweb/worksheetdesign/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control), [com.aspose.gridweb.WebWorksheet](../../com.aspose.gridweb/webworksheet)
```
public class WorksheetDesign extends WebWorksheet
```

Ärvd från WebWorksheet. Används endast under design‑tid.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [WorksheetDesign()](#WorksheetDesign--) | Standardkonstruktor. |
| [WorksheetDesign(MainWeb mw, GridWorksheet gwk)](#WorksheetDesign-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-) | konstruktorn med MainWeb och GridWorksheet |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Anpassar automatiskt kolumnbredden. |
| [autoFitColumn(int columnIndex, int startRow, int endRow)](#autoFitColumn-int-int-int-) | Anpassar automatiskt kolumnbredden. |
| [cancelNewBindRow()](#cancelNewBindRow--) | Avbryter och tar bort den nyss tillagda bindningsraden. |
| [commitNewBindRow()](#commitNewBindRow--) | Bekräftar den nyss tillagda bindningsraden och lägger till den i datakällan. |
| [copy(WebWorksheet source)](#copy-com.aspose.gridweb.WebWorksheet-) | Kopierar från ett annat arbetsbladsobjekt. |
| [createAutoGenratedColumns()](#createAutoGenratedColumns--) | Efter att ha ställt in en datakälla för arbetsbladet, anropa den här metoden för att automatiskt generera bindningskolumnerna. |
| [createNewBindRow()](#createNewBindRow--) | Skapar en ny bindningsrad och binder den till datakällan. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Skapar delsumma i bladet. |
| [dataBind()](#dataBind--) | Bind arbetsbladet till datakällan. |
| [deleteBindRow(int rowNum)](#deleteBindRow-int-) | Tar bort en bindningsrad. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Fryser rutor vid den angivna cellen i kalkylbladet. |
| [getBindStartColumn()](#getBindStartColumn--) | I datakopplingsläge indikerar BindStartRow och BindStartColumn positionen för rutnätet som ska bindas till datakällan. |
| [getBindStartRow()](#getBindStartRow--) | I datakopplingsläge indikerar BindStartRow och BindStartColumn positionen för rutnätet som ska bindas till datakällan. |
| [getBindingSource()](#getBindingSource--) | Det faktiska bindnings‑datakällobjektet vid körning. |
| [getClass()](#getClass--) |  |
| [getCurrentBindRows()](#getCurrentBindRows--) | Hämtar antalet bindningsrader i data-bindningsläge. |
| [getDataMember()](#getDataMember--) | Hämtar DataMember från den flermedlems DataSource. |
| [getDataSource()](#getDataSource--) | Hämtar DataSource. |
| [getEnableCreateBindColumnHeader()](#getEnableCreateBindColumnHeader--) | I data-bindningsläge anger om kolumnrubriktexter ska skapas i bladet. |
| [getIndex()](#getIndex--) | Hämtar sitt eget index bland arbetsbladen. |
| [getName()](#getName--) | Hämtar bladets namn. |
| [getUniqueID()](#getUniqueID--) | Hämtar UniqueID i kontrollen |
| [getValidations()](#getValidations--) | Hämtar samlingen av datavalideringsinställningar i kalkylbladet. |
| [getVisible()](#getVisible--) | Anger om detta bladnamn visas i bladflikarna i kontrollen. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Grupperar rader. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Grupperar rader. |
| [hashCode()](#hashCode--) |  |
| [isProtected()](#isProtected--) | Hämtar om arbetsbladet är skyddat. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllCellsEditable()](#setAllCellsEditable--) | Gör alla celler redigerbara.det är ett utökat attribut |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Gör alla celler skrivskyddade.det är ett utökat attribut observera att detta attribut inte kan behållas i faktiska celler, om du vill behålla skyddet använd setProtect |
| [setBindStartColumn(int value)](#setBindStartColumn-int-) | I datakopplingsläge indikerar BindStartRow och BindStartColumn positionen för rutnätet som ska bindas till datakällan. |
| [setBindStartRow(int value)](#setBindStartRow-int-) | I datakopplingsläge indikerar BindStartRow och BindStartColumn positionen för rutnätet som ska bindas till datakällan. |
| [setCurrentBindRows(int value)](#setCurrentBindRows-int-) | Hämtar antalet bindningsrader i data-bindningsläge. |
| [setDataMember(String value)](#setDataMember-java.lang.String-) | Ställer in DataMember från den flermedlems DataSource. |
| [setDataSource(Object value)](#setDataSource-java.lang.Object-) | Ställer in DataSource. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Gör ett område av celler redigerbara. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Gör alla celler skrivskyddade genom att anropa SetAllCellsReadonly method. |
| [setEnableCreateBindColumnHeader(boolean value)](#setEnableCreateBindColumnHeader-boolean-) | I data-bindningsläge anger om kolumnrubriktexter ska skapas i bladet. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in bladets namn. |
| [setProtected(boolean value)](#setProtected-boolean-) | Ställer in om arbetsbladet är skyddat. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Gör ett område av celler skrivskyddade. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells First make all cells editable by calling the SetAllCellsEditable method. |
| [setVisible(boolean value)](#setVisible-boolean-) | Anger om detta bladnamn visas i bladflikarna i kontrollen. |
| [toString()](#toString--) |  |
| [unfreezePanes()](#unfreezePanes--) | Låser upp paneler i kalkylbladet. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Avgrupperar rader. |
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


konstruktorn med MainWeb och GridWorksheet

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mw | [MainWeb](../../com.aspose.gridweb/mainweb) |  |
| gwk | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) |  |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Anpassar automatiskt kolumnbredden.

**Remarks**

AutoFitColumn är en inexakt funktion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | Kolumnindex. |

### autoFitColumn(int columnIndex, int startRow, int endRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int startRow, int endRow)
```


Automatiserar kolumnbredden. Denna metod anpassar en kolumn baserat på innehållet i ett cellintervall inom kolumnen från startRow till endRow. AutoFitColumn är en inexakt funktion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | int | kolumnindex, nollbaserat |
| startRad | int | startradindex, nollbaserat |
| slutRad | int | slutradindex, nollbaserat |

### cancelNewBindRow() {#cancelNewBindRow--}
```
public int cancelNewBindRow()
```


Avbryter och tar bort den nyss tillagda bindningsraden.

**Returns:**
int – radindexet. Om ingen ny bindningsrad har skapats returneras -1.
### commitNewBindRow() {#commitNewBindRow--}
```
public int commitNewBindRow()
```


Bekräftar den nyss tillagda bindningsraden och lägger till den i datakällan.

**Returns:**
int – radindexet för den nya raden. Om ingen rad skapas returneras -1.
### copy(WebWorksheet source) {#copy-com.aspose.gridweb.WebWorksheet-}
```
public void copy(WebWorksheet source)
```


Kopierar från ett annat arbetsbladsobjekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [WebWorksheet](../../com.aspose.gridweb/webworksheet) | Det andra bladet. |

### createAutoGenratedColumns() {#createAutoGenratedColumns--}
```
public void createAutoGenratedColumns()
```


Efter att ha ställt in en datakälla för arbetsbladet, anropa den här metoden för att automatiskt generera bindningskolumnerna.

### createNewBindRow() {#createNewBindRow--}
```
public int createNewBindRow()
```


Skapar en ny bindningsrad och binder den till datakällan.

**Returns:**
int – radindexet för den nya raden. Om ingen rad skapas returneras -1.
### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


Skapar delsumma i bladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnNameRowIndex | int | Radindex för kolumnnamnsraden. |
| dataRows | int | Antalet datarader. |
| groupByColumnIndex | int | Kolumnindex för den kolumn som ska grupperas. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Subtotal-funktionstypen. |
| subtotalColumnIndexList | int[] | Kolumnindex som ska summeras. |
| functionLabel | java.lang.String | Etiketten för subtotalfunktionen. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Stilen för totalraden. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Stilen för subtotalraden. |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype). Nummertypen för subtotalresultatcellerna. |
| customString | java.lang.String | Den anpassade formatsträngen för subtotalresultatcellerna. Kan vara null. |

### dataBind() {#dataBind--}
```
public void dataBind()
```


Bind arbetsbladet till datakällan.

### deleteBindRow(int rowNum) {#deleteBindRow-int-}
```
public int deleteBindRow(int rowNum)
```


Tar bort en bindningsrad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowNum | int | Radindexet. |

**Returns:**
int – index för den raderade raden. Om ingen bindningsrad raderas returneras -1.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Fryser rutor vid den angivna cellen i kalkylbladet.

**Remarks**

Radindex och kolumnindex kan inte alla vara noll. Antalet rader och antalet kolumner kan inte heller alla vara noll.

De två första parametrarna anger den frysta positionen och de två sista parametrarna anger området som är fryst i det övre vänstra fönstret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| kolumn | int | Kolumnindex. |
| freezedRows | int | Antal synliga rader i övre fönstret, högst lika med radindex. |
| freezedColumns | int | Antalet synliga kolumner i vänsterpanelen, högst kolumnindexet. |

### getBindStartColumn() {#getBindStartColumn--}
```
public int getBindStartColumn()
```


I datakopplingsläge indikerar BindStartRow och BindStartColumn positionen för rutnätet som ska bindas till datakällan.

**Returns:**
int
### getBindStartRow() {#getBindStartRow--}
```
public int getBindStartRow()
```


I datakopplingsläge indikerar BindStartRow och BindStartColumn positionen för rutnätet som ska bindas till datakällan.

**Returns:**
int
### getBindingSource() {#getBindingSource--}
```
public Iterable getBindingSource()
```


Det faktiska bindningsdatasource-objektet vid körning. Det är ett DataView-objekt när DataSource‑egenskapen är ett DataSet-, DataTable- eller DataView‑objekt.

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


Hämtar antalet bindningsrader i data-bindningsläge.

**Returns:**
int
### getDataMember() {#getDataMember--}
```
public String getDataMember()
```


Hämtar DataMember från den flermedlems DataSource. Vanligtvis representerar det ett DataTable‑objekt i ett DataSet.

**Returns:**
java.lang.String
### getDataSource() {#getDataSource--}
```
public Object getDataSource()
```


Hämtar DataSource. Vanligtvis är det ett DataSet‑objekt.

**Returns:**
java.lang.Object
### getEnableCreateBindColumnHeader() {#getEnableCreateBindColumnHeader--}
```
public boolean getEnableCreateBindColumnHeader()
```


I data-bindningsläge anger om kolumnrubriktexter ska skapas i bladet.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


Hämtar sitt eget index bland arbetsbladen.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Hämtar bladets namn.

**Returns:**
java.lang.String
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Hämtar UniqueID i kontrollen

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


Hämtar samlingen av datavalideringsinställningar i kalkylbladet.

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Anger om detta bladnamn visas i bladflikarna i kontrollen.

**Returns:**
boolean
### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Grupperar rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första radindexet som ska grupperas. |
| lastIndex | int | Det sista radindexet som ska grupperas. |

### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Grupperar rader.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första radindexet som ska grupperas. |
| lastIndex | int | Det sista radindexet som ska grupperas. |
| isHidden | boolean | Anger om de grupperade raderna är dolda. |

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


Hämtar om arbetsbladet är skyddat. När ett arbetsblad är skyddat kan inte alla celler redigeras förutom de celler vars IsLocked‑egenskap är falsk.

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


Gör alla celler redigerbara.det är ett utökat attribut

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


Gör alla celler skrivskyddade.det är ett utökat attribut observera att detta attribut inte kan behållas i faktiska celler, om du vill behålla skyddet använd setProtect

### setBindStartColumn(int value) {#setBindStartColumn-int-}
```
public void setBindStartColumn(int value)
```


I datakopplingsläge indikerar BindStartRow och BindStartColumn positionen för rutnätet som ska bindas till datakällan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBindStartRow(int value) {#setBindStartRow-int-}
```
public void setBindStartRow(int value)
```


I datakopplingsläge indikerar BindStartRow och BindStartColumn positionen för rutnätet som ska bindas till datakällan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setCurrentBindRows(int value) {#setCurrentBindRows-int-}
```
public void setCurrentBindRows(int value)
```


Hämtar antalet bindningsrader i data-bindningsläge.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setDataMember(String value) {#setDataMember-java.lang.String-}
```
public void setDataMember(String value)
```


Ställer in DataMember från den flermedlems DataSource. Vanligtvis representerar det ett DataTable‑objekt i ett DataSet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDataSource(Object value) {#setDataSource-java.lang.Object-}
```
public void setDataSource(Object value)
```


Ställer in DataSource. Vanligtvis är det ett DataSet‑objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


Gör ett cellområde redigerbart. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Gör alla celler skrivskyddade genom att anropa metoden SetAllCellsReadonly. Anropa sedan den här metoden för att ange vilka celler som ska vara redigerbara

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startraden för intervallet. |
| startColumn | int | Startkolumnen för intervallet. |
| rader | int | Antalet rader. |
| kolumner | int | Antalet kolumner. |

### setEnableCreateBindColumnHeader(boolean value) {#setEnableCreateBindColumnHeader-boolean-}
```
public void setEnableCreateBindColumnHeader(boolean value)
```


I data-bindningsläge anger om kolumnrubriktexter ska skapas i bladet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in bladets namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setProtected(boolean value) {#setProtected-boolean-}
```
public void setProtected(boolean value)
```


Ställer in om kalkylbladet är skyddat. När ett kalkylblad är skyddat kan inte alla celler redigeras förutom den cell vars IsLocked property är falsk.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


Gör ett cellområde readonly. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Gör först alla celler redigerbara genom att anropa metoden SetAllCellsEditable. Anropa sedan den här metoden för för att ange vilka celler som ska vara readonly

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startraden för intervallet. |
| startColumn | int | Startkolumnen för intervallet. |
| rader | int | Antalet rader. |
| kolumner | int | Antalet kolumner. |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Anger om detta bladnamn visas i bladflikarna i kontrollen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

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


Låser upp paneler i kalkylbladet.

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Avgrupperar rader.

**Remarks**

Tar bara bort yttre gruppinformation.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstIndex | int | Det första radindexet som ska avgrupperas. |
| lastIndex | int | Det sista radindexet som ska avgrupperas. |

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

