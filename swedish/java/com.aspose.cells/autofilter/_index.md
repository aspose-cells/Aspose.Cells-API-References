---
title: "AutoFilter"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar autofilter för det angivna kalkylbladet."
type: docs
url: /sv/java/com.aspose.cells/autofilter/
---

**Inheritance:**
java.lang.Object
```
public class AutoFilter
```

Representerar autofilter för det angivna kalkylbladet.

**Example**

```
         //Creating a file stream containing the Excel file to be opened
         //Instantiating a Workbook object
         Workbook workbook = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating AutoFilter by giving the cells range of the heading row
         worksheet.getAutoFilter().setRange("A1:B1");
         //Filtering columns with specified values
         worksheet.getAutoFilter().filter(1, "Bananas");
         //Saving the modified Excel file.
         workbook.save("output.xls");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#addDateFilter-int-int-int-int-int-int-int-int-) | Lägger till ett datumfilter. |
| [addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)](#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-) | Lägger till ett fyllnadsfärgsfilter. |
| [addFilter(int fieldIndex, String criteria)](#addFilter-int-java.lang.String-) | Lägger till ett filter för en filterkolumn. |
| [addFontColorFilter(int fieldIndex, CellsColor color)](#addFontColorFilter-int-com.aspose.cells.CellsColor-) | Lägger till ett teckensnittsfärgsfilter. |
| [addIconFilter(int fieldIndex, int iconSetType, int iconId)](#addIconFilter-int-int-int-) | Lägger till ett ikonfilter. |
| [custom(int fieldIndex, int operatorType1, Object criteria1)](#custom-int-int-java.lang.Object-) | Filtrerar en lista med ett anpassat kriterium. |
| [custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-) | Filtrerar en lista med anpassade kriterier. |
| [dynamicFilter(int fieldIndex, int dynamicFilterType)](#dynamicFilter-int-int-) | Lägger till ett dynamiskt filter. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int fieldIndex, String criteria)](#filter-int-java.lang.String-) | Filtrerar en lista med angivna kriterier. |
| [filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)](#filterTop10-int-boolean-boolean-int-) | Filtrera de 10 översta objekten i listan |
| [getCellArea()](#getCellArea--) | Hämtar [CellArea](../../com.aspose.cells/cellarea) där detta AutoFilter gäller. |
| [getCellArea(boolean refreshAppliedRange)](#getCellArea-boolean-) | Hämtar [CellArea](../../com.aspose.cells/cellarea) där det angivna AutoFiltret gäller. |
| [getClass()](#getClass--) |  |
| [getFilterColumns()](#getFilterColumns--) | Hämtar samlingen av filterkolumnerna. |
| [getRange()](#getRange--) | Representerar intervallet som det angivna AutoFiltret gäller för. |
| [getShowFilterButton()](#getShowFilterButton--) | Anger om AutoFilter‑knappen för den här kolumnen är synlig. |
| [getSorter()](#getSorter--) | Hämtar datasorteringen. |
| [hashCode()](#hashCode--) |  |
| [matchBlanks(int fieldIndex)](#matchBlanks-int-) | Matcha alla tomma celler i listan. |
| [matchNonBlanks(int fieldIndex)](#matchNonBlanks-int-) | Matcha alla icke-tomma celler i listan. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Uppdatera autofilter för att dölja eller visa raderna. |
| [refresh(boolean hideRows)](#refresh-boolean-) | Hämtar alla dolda raders index. |
| [removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#removeDateFilter-int-int-int-int-int-int-int-int-) | Tar bort ett datumfilter. |
| [removeFilter(int fieldIndex)](#removeFilter-int-) | Ta bort det specifika filtret. |
| [removeFilter(int fieldIndex, String criteria)](#removeFilter-int-java.lang.String-) | Tar bort ett filter för en filterkolumn. |
| [setRange(int row, int startColumn, int endColumn)](#setRange-int-int-int-) | Ställer in intervallet som det angivna AutoFiltret gäller för. |
| [setRange(String value)](#setRange-java.lang.String-) | Representerar intervallet som det angivna AutoFiltret gäller för. |
| [setShowFilterButton(boolean value)](#setShowFilterButton-boolean-) | Anger om AutoFilter‑knappen för den här kolumnen är synlig. |
| [showAll()](#showAll--) | Visa alla rader. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#addDateFilter-int-int-int-int-int-int-int-int-}
```
public void addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Lägger till ett datumfilter.

**Remarks**

Om DateTimeGroupingType är Year, påverkas endast parametern year. Om DateTiemGroupingType är Month, påverkas endast parametrarna year och month.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstremsta fältet är fält 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Gruppindelningstypen |
| år | int | Året. |
| månad | int | Månad. |
| dag | int | Dag. |
| timme | int | Timmen. |
| minut | int | Minuten. |
| sekund | int | Sekunden. |

### addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor) {#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-}
```
public void addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)
```


Lägger till ett fyllnadsfärgsfilter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstremsta fältet är fält 0). |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). Bakgrundsmönsterstypen. |
| foregroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | Förgrundsfärgen. |
| backgroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | Bakgrundsfärgen. |

### addFilter(int fieldIndex, String criteria) {#addFilter-int-java.lang.String-}
```
public void addFilter(int fieldIndex, String criteria)
```


Lägger till ett filter för en filterkolumn.

**Remarks**

MS Excel 2007 stöder flera val i en filterkolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstremsta fältet är fält 0). |
| kriterier | java.lang.String | Det angivna kriteriet (en sträng; till exempel "101"). Det kan bara vara null eller vara ett av cellernas värde i den här kolumnen. |

### addFontColorFilter(int fieldIndex, CellsColor color) {#addFontColorFilter-int-com.aspose.cells.CellsColor-}
```
public void addFontColorFilter(int fieldIndex, CellsColor color)
```


Lägger till ett teckensnittsfärgsfilter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstremsta fältet är fält 0). |
| color | [CellsColor](../../com.aspose.cells/cellscolor) | Objektet [CellsColor](../../com.aspose.cells/cellscolor). |

### addIconFilter(int fieldIndex, int iconSetType, int iconId) {#addIconFilter-int-int-int-}
```
public void addIconFilter(int fieldIndex, int iconSetType, int iconId)
```


Lägger till ett ikonfilter.

**Remarks**

Stöder endast att lägga till ikonfilter. Stöder inte att kontrollera vilken rad som är synlig om filtret är ett ikonfilter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstremsta fältet är fält 0). |
| iconSetType | int | [IconSetType](../../com.aspose.cells/iconsettype). Ikonsettyp. |
| iconId | int | Ikon‑id‑t. |

### custom(int fieldIndex, int operatorType1, Object criteria1) {#custom-int-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1)
```


Filtrerar en lista med ett anpassat kriterium.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstremsta fältet är fält 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Filteroperatortypen |
| criteria1 | java.lang.Object | Det anpassade kriteriet |

### custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


Filtrerar en lista med anpassade kriterier.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstremsta fältet är fält 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Filteroperatortypen |
| criteria1 | java.lang.Object | Det anpassade kriteriet |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). Filteroperatortypen |
| criteria2 | java.lang.Object | Det anpassade kriteriet |

### dynamicFilter(int fieldIndex, int dynamicFilterType) {#dynamicFilter-int-int-}
```
public void dynamicFilter(int fieldIndex, int dynamicFilterType)
```


Lägger till ett dynamiskt filter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstremsta fältet är fält 0). |
| dynamicFilterType | int | [DynamicFilterType](../../com.aspose.cells/dynamicfiltertype). Dynamisk filtertyp. |

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
### filter(int fieldIndex, String criteria) {#filter-int-java.lang.String-}
```
public void filter(int fieldIndex, String criteria)
```


Filtrerar en lista med angivna kriterier.

**Remarks**

Aspose.Cells kommer att ta bort alla andra filterinställningar på detta fält som i MS Excel 97-2003.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstremsta fältet är fält 0). |
| kriterier | java.lang.String | Det angivna kriteriet (en sträng; till exempel "101"). |

### filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount) {#filterTop10-int-boolean-boolean-int-}
```
public void filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)
```


Filtrera de 10 översta objekten i listan

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstremsta fältet är fält 0). |
| isTop | boolean | Indikerar om filtret är från toppen eller botten. |
| isPercent | boolean | Anger om objekten är procent eller antal |
| itemCount | int | Antalet objekt. |

### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Hämtar [CellArea](../../com.aspose.cells/cellarea) där detta AutoFilter gäller.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getCellArea(boolean refreshAppliedRange) {#getCellArea-boolean-}
```
public CellArea getCellArea(boolean refreshAppliedRange)
```


Hämtar [CellArea](../../com.aspose.cells/cellarea) där det angivna AutoFiltret gäller.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| refreshAppliedRange | boolean | Om det tillämpade intervallet ska uppdateras. För det tillämpade intervallet för autofilter kan den sista raden ändras när celldata ändras. Om detta flagga är sann, beräknas den sista raden i intervallet om enligt aktuell celldata. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilterColumns() {#getFilterColumns--}
```
public FilterColumnCollection getFilterColumns()
```


Hämtar samlingen av filterkolumnerna.

**Returns:**
[FilterColumnCollection](../../com.aspose.cells/filtercolumncollection)
### getRange() {#getRange--}
```
public String getRange()
```


Representerar intervallet som det angivna AutoFiltret gäller för.

**Returns:**
java.lang.String
### getShowFilterButton() {#getShowFilterButton--}
```
public boolean getShowFilterButton()
```


Anger om AutoFilter‑knappen för den här kolumnen är synlig.

**Returns:**
boolean
### getSorter() {#getSorter--}
```
public DataSorter getSorter()
```


Hämtar datasorteringen.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### matchBlanks(int fieldIndex) {#matchBlanks-int-}
```
public void matchBlanks(int fieldIndex)
```


Matcha alla tomma celler i listan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstremsta fältet är fält 0). |

### matchNonBlanks(int fieldIndex) {#matchNonBlanks-int-}
```
public void matchNonBlanks(int fieldIndex)
```


Matcha alla icke-tomma celler i listan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstremsta fältet är fält 0). |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public int[] refresh()
```


Uppdatera autofilter för att dölja eller visa raderna.

**Returns:**
int[] - Returnerar alla dolda radernas index.
### refresh(boolean hideRows) {#refresh-boolean-}
```
public int[] refresh(boolean hideRows)
```


Hämtar alla dolda raders index.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| hideRows | boolean | Om true, dölj de filtrerade raderna. |

**Returns:**
int[] - Returnerar alla dolda radernas index.
### removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#removeDateFilter-int-int-int-int-int-int-int-int-}
```
public void removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


Tar bort ett datumfilter.

**Remarks**

Om DateTimeGroupingType är Year, påverkas endast parametern year. Om DateTiemGroupingType är Month, påverkas endast parametrarna year och month.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstremsta fältet är fält 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Gruppindelningstypen |
| år | int | Året. |
| månad | int | Månad. |
| dag | int | Dag. |
| timme | int | Timmen. |
| minut | int | Minuten. |
| sekund | int | Sekunden. |

### removeFilter(int fieldIndex) {#removeFilter-int-}
```
public void removeFilter(int fieldIndex)
```


Ta bort det specifika filtret.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det specifika filterindexet |

### removeFilter(int fieldIndex, String criteria) {#removeFilter-int-java.lang.String-}
```
public void removeFilter(int fieldIndex, String criteria)
```


Tar bort ett filter för en filterkolumn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | Det heltalsavståndet för fältet som du vill basera filtret på (från listans vänstra sida; det vänstremsta fältet är fält 0). |
| kriterier | java.lang.String | Det angivna kriteriet (en sträng; till exempel "101"). Det kan bara vara null eller vara ett av cellernas värde i den här kolumnen. |

### setRange(int row, int startColumn, int endColumn) {#setRange-int-int-int-}
```
public void setRange(int row, int startColumn, int endColumn)
```


Ställer in intervallet som det angivna AutoFiltret gäller för.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Radindex. |
| startColumn | int | Startkolumnens index. |
| endColumn | int | Slutkolumnindex. |

### setRange(String value) {#setRange-java.lang.String-}
```
public void setRange(String value)
```


Representerar intervallet som det angivna AutoFiltret gäller för.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setShowFilterButton(boolean value) {#setShowFilterButton-boolean-}
```
public void setShowFilterButton(boolean value)
```


Anger om AutoFilter‑knappen för den här kolumnen är synlig.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### showAll() {#showAll--}
```
public void showAll()
```


Visa alla rader.

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

