---
title: "ListObject"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en tabell i ett kalkylblad."
type: docs
url: /sv/java/com.aspose.cells/listobject/
---

**Inheritance:**
java.lang.Object
```
public class ListObject
```

Representerar en tabell i ett kalkylblad.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         for (int i = 0; i  ? i++)
         {
         cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
          }
         for (int row = 1; row  ? row++)
         {
          for (int column = 0; column  ? column++)
         {
         cells.get(row, column).putValue(row * column);
          }
          }
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setShowTotals(true);
         table.getListColumns().get(4).setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
         workbook.save("Book1.xlsx");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [applyStyleToRange()](#applyStyleToRange--) | Applicera tabellstilen på området. |
| [convertToRange()](#convertToRange--) | Konvertera tabellen till ett område. |
| [convertToRange(TableToRangeOptions options)](#convertToRange-com.aspose.cells.TableToRangeOptions-) | Konvertera tabellen till ett område. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter()](#filter--) | Filtrera tabellen. |
| [getAlternativeDescription()](#getAlternativeDescription--) | Hämtar den alternativa beskrivningen. |
| [getAlternativeText()](#getAlternativeText--) | Hämtar den alternativa texten. |
| [getAutoFilter()](#getAutoFilter--) | Hämtar autofiltret för den här tabellen. |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Hämtar kommentaren för tabellen. |
| [getDataRange()](#getDataRange--) | Hämtar dataområdet för tabellen. |
| [getDataSourceType()](#getDataSourceType--) | Hämtar datakälltyp för tabellen. |
| [getDisplayName()](#getDisplayName--) | Hämtar tabellens visningsnamn. |
| [getEndColumn()](#getEndColumn--) | Hämtar slutkolumnen för intervallet. |
| [getEndRow()](#getEndRow--) | Hämtar slutraden för intervallet. |
| [getListColumns()](#getListColumns--) | Hämtar [ListColumn](../../com.aspose.cells/listcolumn)-listan för den här tabellen. |
| [getQueryTable()](#getQueryTable--) | Hämtar den länkade QueryTable. |
| [getShowHeaderRow()](#getShowHeaderRow--) | Hämtar om den här tabellen visar rubrikrad. |
| [getShowTableStyleColumnStripes()](#getShowTableStyleColumnStripes--) | Indikerar om kolumnrandig formatering har tillämpats. |
| [getShowTableStyleFirstColumn()](#getShowTableStyleFirstColumn--) | Indikerar om den första kolumnen i tabellen har den tillämpade stilen. |
| [getShowTableStyleLastColumn()](#getShowTableStyleLastColumn--) | Indikerar om den sista kolumnen i tabellen har den tillämpade stilen. |
| [getShowTableStyleRowStripes()](#getShowTableStyleRowStripes--) | Indikerar om radrandig formatering har tillämpats. |
| [getShowTotals()](#getShowTotals--) | Hämtar om den här tabellen visar totalsrad. |
| [getStartColumn()](#getStartColumn--) | Hämtar startkolumnen för intervallet. |
| [getStartRow()](#getStartRow--) | Hämtar startraden för intervallet. |
| [getTableStyleName()](#getTableStyleName--) | Hämtar tabellens stilnamn. |
| [getTableStyleType()](#getTableStyleType--) | Hämtar den inbyggda tabellstilen. |
| [getXmlMap()](#getXmlMap--) | Hämtar en [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) som används för den här listan. |
| [hasAutoFilter()](#hasAutoFilter--) | Indikerar om autofilter har tillämpats på den här tabellen. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putCellFormula(int rowOffset, int columnOffset, String formula)](#putCellFormula-int-int-java.lang.String-) | Sätt formeln i cellen i tabellen. |
| [putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)](#putCellFormula-int-int-java.lang.String-boolean-) | Sätt formeln i cellen i tabellen. |
| [putCellValue(int rowOffset, int columnOffset, Object value)](#putCellValue-int-int-java.lang.Object-) | Sätt värdet i cellen. |
| [putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)](#putCellValue-int-int-java.lang.Object-boolean-) | Sätt värdet i cellen. |
| [removeAutoFilter()](#removeAutoFilter--) | Tar bort autofilter som har tillämpats på den här tabellen. |
| [resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)](#resize-int-int-int-int-boolean-) | Ändra storlek på intervallet för listobjektet. |
| [setAlternativeDescription(String value)](#setAlternativeDescription-java.lang.String-) | Ställer in den alternativa beskrivningen. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Ställer in den alternativa texten. |
| [setComment(String value)](#setComment-java.lang.String-) | Ställer in kommentaren för tabellen. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Ställer in tabellens visningsnamn. |
| [setHasAutoFilter(boolean value)](#setHasAutoFilter-boolean-) | Indikerar om autofilter har tillämpats på den här tabellen. |
| [setShowHeaderRow(boolean value)](#setShowHeaderRow-boolean-) | Ställer in om den här tabellen visar rubrikrad. |
| [setShowTableStyleColumnStripes(boolean value)](#setShowTableStyleColumnStripes-boolean-) | Indikerar om kolumnrandig formatering har tillämpats. |
| [setShowTableStyleFirstColumn(boolean value)](#setShowTableStyleFirstColumn-boolean-) | Indikerar om den första kolumnen i tabellen har den tillämpade stilen. |
| [setShowTableStyleLastColumn(boolean value)](#setShowTableStyleLastColumn-boolean-) | Indikerar om den sista kolumnen i tabellen har den tillämpade stilen. |
| [setShowTableStyleRowStripes(boolean value)](#setShowTableStyleRowStripes-boolean-) | Indikerar om radrandig formatering har tillämpats. |
| [setShowTotals(boolean value)](#setShowTotals-boolean-) | Ställer in om detta TAble visar totalrad. |
| [setTableStyleName(String value)](#setTableStyleName-java.lang.String-) | Ställer in tabellens stilnamn. |
| [setTableStyleType(int value)](#setTableStyleType-int-) | Hämtar den inbyggda tabellstilen. |
| [toString()](#toString--) |  |
| [updateColumnName()](#updateColumnName--) | Uppdaterar alla listkolumners namn till celler i tabellen. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyleToRange() {#applyStyleToRange--}
```
public void applyStyleToRange()
```


Applicera tabellstilen på området.

### convertToRange() {#convertToRange--}
```
public void convertToRange()
```


Konvertera tabellen till ett område.

### convertToRange(TableToRangeOptions options) {#convertToRange-com.aspose.cells.TableToRangeOptions-}
```
public void convertToRange(TableToRangeOptions options)
```


Konvertera tabellen till ett område.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| options | [TableToRangeOptions](../../com.aspose.cells/tabletorangeoptions) | alternativen när tabellen konverteras till ett område. |

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
### filter() {#filter--}
```
public AutoFilter filter()
```


Filtrera tabellen.

**Remarks**

OBS: Denna medlem är nu föråldrad. Istället, vänligen sätt ListObject.HasAutoFilter-egenskapen./// Denna egenskap kommer att tas bort 12 månader senare från och med oktober 2025. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getAlternativeDescription() {#getAlternativeDescription--}
```
public String getAlternativeDescription()
```


Hämtar den alternativa beskrivningen.

**Returns:**
java.lang.String
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Hämtar den alternativa texten.

**Returns:**
java.lang.String
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Hämtar autofiltret för den här tabellen.

**Remarks**

Det fungerar endast när [hasAutoFilter()](../../com.aspose.cells/listobject\#hasAutoFilter--) är falskt.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComment() {#getComment--}
```
public String getComment()
```


Hämtar kommentaren för tabellen.

**Returns:**
java.lang.String
### getDataRange() {#getDataRange--}
```
public Range getDataRange()
```


Hämtar dataområdet för tabellen.

**Returns:**
[Range](../../com.aspose.cells/range)
### getDataSourceType() {#getDataSourceType--}
```
public int getDataSourceType()
```


Hämtar datakälltyp för tabellen.

Se [TableDataSourceType](../../com.aspose.cells/tabledatasourcetype).

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Hämtar tabellens visningsnamn.

**Returns:**
java.lang.String
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Hämtar slutkolumnen för intervallet.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Hämtar slutraden för intervallet.

**Returns:**
int
### getListColumns() {#getListColumns--}
```
public ListColumnCollection getListColumns()
```


Hämtar [ListColumn](../../com.aspose.cells/listcolumn)-listan för den här tabellen.

**Returns:**
[ListColumnCollection](../../com.aspose.cells/listcolumncollection)
### getQueryTable() {#getQueryTable--}
```
public QueryTable getQueryTable()
```


Hämtar den länkade QueryTable.

**Returns:**
[QueryTable](../../com.aspose.cells/querytable)
### getShowHeaderRow() {#getShowHeaderRow--}
```
public boolean getShowHeaderRow()
```


Hämtar om den här tabellen visar rubrikrad.

**Returns:**
boolean
### getShowTableStyleColumnStripes() {#getShowTableStyleColumnStripes--}
```
public boolean getShowTableStyleColumnStripes()
```


Indikerar om kolumnrandig formatering har tillämpats.

**Returns:**
boolean
### getShowTableStyleFirstColumn() {#getShowTableStyleFirstColumn--}
```
public boolean getShowTableStyleFirstColumn()
```


Indikerar om den första kolumnen i tabellen har den tillämpade stilen.

**Returns:**
boolean
### getShowTableStyleLastColumn() {#getShowTableStyleLastColumn--}
```
public boolean getShowTableStyleLastColumn()
```


Indikerar om den sista kolumnen i tabellen har den tillämpade stilen.

**Returns:**
boolean
### getShowTableStyleRowStripes() {#getShowTableStyleRowStripes--}
```
public boolean getShowTableStyleRowStripes()
```


Indikerar om radrandig formatering har tillämpats.

**Returns:**
boolean
### getShowTotals() {#getShowTotals--}
```
public boolean getShowTotals()
```


Hämtar om den här tabellen visar totalsrad.

**Returns:**
boolean
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Hämtar startkolumnen för intervallet.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Hämtar startraden för intervallet.

**Returns:**
int
### getTableStyleName() {#getTableStyleName--}
```
public String getTableStyleName()
```


Hämtar tabellens stilnamn.

**Returns:**
java.lang.String
### getTableStyleType() {#getTableStyleType--}
```
public int getTableStyleType()
```


Hämtar den inbyggda tabellstilen.

Se [TableStyleType](../../com.aspose.cells/tablestyletype).

**Example**

```
         Workbook workbook = new Workbook("Book1.xlsx");
         ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
         int index = tables.add(0, 0, 9, 4, true);
         ListObject table = tables.get(0);
         table.setTableStyleType(TableStyleType.TABLE_STYLE_DARK_2);
          workbook.save("TableStyle.xlsx");
```

**Returns:**
int
### getXmlMap() {#getXmlMap--}
```
public XmlMap getXmlMap()
```


Hämtar en [getXmlMap()](../../com.aspose.cells/listobject\#getXmlMap--) som används för den här listan.

**Returns:**
[XmlMap](../../com.aspose.cells/xmlmap)
### hasAutoFilter() {#hasAutoFilter--}
```
public boolean hasAutoFilter()
```


Indikerar om autofilter har tillämpats på den här tabellen.

**Returns:**
boolean
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




### putCellFormula(int rowOffset, int columnOffset, String formula) {#putCellFormula-int-int-java.lang.String-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula)
```


Sätt formeln i cellen i tabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | int | Radavståndet i tabellen. |
| columnOffset | int | Kolumnavståndet i tabellen. |
| formula | java.lang.String | Formeln för cellen. |

### putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula) {#putCellFormula-int-int-java.lang.String-boolean-}
```
public void putCellFormula(int rowOffset, int columnOffset, String formula, boolean isTotalsRowFormula)
```


Sätt formeln i cellen i tabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | int | Radavståndet i tabellen. |
| columnOffset | int | Kolumnavståndet i tabellen. |
| formula | java.lang.String | Formeln för cellen. |
| isTotalsRowFormula | boolean |  |

### putCellValue(int rowOffset, int columnOffset, Object value) {#putCellValue-int-int-java.lang.Object-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value)
```


Sätt värdet i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | int | Radavståndet i tabellen. |
| columnOffset | int | Kolumnavståndet i tabellen. |
| värde | java.lang.Object | Cellvärdet. |

### putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel) {#putCellValue-int-int-java.lang.Object-boolean-}
```
public void putCellValue(int rowOffset, int columnOffset, Object value, boolean isTotalsRowLabel)
```


Sätt värdet i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowOffset | int | Radavståndet i tabellen. |
| columnOffset | int | Kolumnavståndet i tabellen. |
| värde | java.lang.Object | Cellvärdet. |
| isTotalsRowLabel | boolean | Anger om det är en etikett för totalrad, fungerar endast för totalrad. Om False och denna rad är totalrad, kommer en ny rad att infogas. |

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Tar bort autofilter som har tillämpats på den här tabellen.

### resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders) {#resize-int-int-int-int-boolean-}
```
public void resize(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders)
```


Ändra storlek på intervallet för listobjektet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startradens index för det nya området. |
| startColumn | int | Startkolumnens index för det nya området. |
| slutRad | int | Slutradens index för det nya området. |
| endColumn | int | Slutkolumnens index för det nya området. |
| hasHeaders | boolean | Om den här tabellen har rubriker. |

### setAlternativeDescription(String value) {#setAlternativeDescription-java.lang.String-}
```
public void setAlternativeDescription(String value)
```


Ställer in den alternativa beskrivningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Ställer in den alternativa texten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```


Ställer in kommentaren för tabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Ställer in tabellens visningsnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setHasAutoFilter(boolean value) {#setHasAutoFilter-boolean-}
```
public void setHasAutoFilter(boolean value)
```


Indikerar om autofilter har tillämpats på den här tabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowHeaderRow(boolean value) {#setShowHeaderRow-boolean-}
```
public void setShowHeaderRow(boolean value)
```


Ställer in om den här tabellen visar rubrikrad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowTableStyleColumnStripes(boolean value) {#setShowTableStyleColumnStripes-boolean-}
```
public void setShowTableStyleColumnStripes(boolean value)
```


Indikerar om kolumnrandig formatering har tillämpats.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowTableStyleFirstColumn(boolean value) {#setShowTableStyleFirstColumn-boolean-}
```
public void setShowTableStyleFirstColumn(boolean value)
```


Indikerar om den första kolumnen i tabellen har den tillämpade stilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowTableStyleLastColumn(boolean value) {#setShowTableStyleLastColumn-boolean-}
```
public void setShowTableStyleLastColumn(boolean value)
```


Indikerar om den sista kolumnen i tabellen har den tillämpade stilen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowTableStyleRowStripes(boolean value) {#setShowTableStyleRowStripes-boolean-}
```
public void setShowTableStyleRowStripes(boolean value)
```


Indikerar om radrandig formatering har tillämpats.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setShowTotals(boolean value) {#setShowTotals-boolean-}
```
public void setShowTotals(boolean value)
```


Ställer in om detta TAble visar totalrad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTableStyleName(String value) {#setTableStyleName-java.lang.String-}
```
public void setTableStyleName(String value)
```


Ställer in tabellens stilnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTableStyleType(int value) {#setTableStyleType-int-}
```
public void setTableStyleType(int value)
```


Hämtar den inbyggda tabellstilen.

Se [TableStyleType](../../com.aspose.cells/tablestyletype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateColumnName() {#updateColumnName--}
```
public void updateColumnName()
```


Uppdaterar alla listkolumners namn till celler i tabellen.

**Remarks**

Värdet på cellerna i tabellens rubrikrad måste vara samma som namnet på ListColumn; Cell.PutValue ändrar inte automatiskt namnet på ListColumn för prestanda.

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

