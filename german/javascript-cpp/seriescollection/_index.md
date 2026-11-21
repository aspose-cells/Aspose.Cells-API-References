---
title: SeriesCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates a collection of Series..series objects.
type: docs
url: /de/javascript-cpp/seriescollection/
---

## SeriesCollection class

Encapsulates a collection of [Series](../series/) objects.

```javascript
class SeriesCollection;
```


### Example
```javascript
const { Workbook, ChartType, SaveFormat } = AsposeCells;

//Instanziieren eines Workbook-Objekts
var workbook = new Workbook();
//Hinzufügen eines neuen Arbeitsblatts zum Excel-Objekt
var sheetIndex = workbook.worksheets.add();
//Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
var worksheet = workbook.worksheets.get(sheetIndex);
//Hinzufügen eines Beispielwerts zur Zelle "A1"
worksheet.cells.get("A1").putValue(50);
//Hinzufügen eines Beispielwerts zur Zelle "A2"
worksheet.cells.get("A2").putValue(100);
//Hinzufügen eines Beispielwerts zur Zelle "A3"
worksheet.cells.get("A3").putValue(150);
//Hinzufügen eines Beispielwerts zur Zelle "A4"
worksheet.cells.get("A4").putValue(200);
//Hinzufügen eines Beispielwerts zur Zelle "B1"
worksheet.cells.get("B1").putValue(60);
//Hinzufügen eines Beispielwerts zur Zelle "B2"
worksheet.cells.get("B2").putValue(32);
//Hinzufügen eines Beispielwerts zur Zelle "B3"
worksheet.cells.get("B3").putValue(50);
//Hinzufügen eines Beispielwerts zur Zelle "B4"
worksheet.cells.get("B4").putValue(40);
//Hinzufügen eines Beispielwerts zur Zelle "C1" als Kategoriedaten
worksheet.cells.get("C1").putValue("Q1");
//Hinzufügen eines Beispielwerts zur Zelle "C2" als Kategoriedaten
worksheet.cells.get("C2").putValue("Q2");
//Hinzufügen eines Beispielwerts zur Zelle "C3" als Kategoriedaten
worksheet.cells.get("C3").putValue("Y1");
//Hinzufügen eines Beispielwerts zur Zelle "C4" als Kategoriedaten
worksheet.cells.get("C4").putValue("Y2");
//Ein Diagramm zum Arbeitsblatt hinzufügen
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Zugriff auf die Instanz des neu hinzugefügten Diagramms
var chart = worksheet.charts.get(chartIndex);
//Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm von der Zelle "A1" bis "B4"
chart.nSeries.add("A1:B4", true);
//Festlegen der Datenquelle für die Kategoriedaten von NSeries
chart.nSeries.categoryData = "C1:C4";
//Speichern der Excel-Datei
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [categoryData](#categoryData--)| string | Gets or sets the range of category Axis values. It can be a range of cells (such as "d1:e10") or a sequence of values (such as "{2,6,8,10}"). |
| [secondCategoryData](#secondCategoryData--)| string | Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some series were plotted on the second axis. |
| [isColorVaried](#isColorVaried--)| boolean | Represents if the color of points is varied. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Series](../series/) element at the specified index. |
| [getSeriesByOrder(number)](#getSeriesByOrder-number-)| Gets the [Series](../series/) element by order. |
| [removeAt(number)](#removeAt-number-)| Remove at a series at the specific index. |
| [changeSeriesOrder(number, number)](#changeSeriesOrder-number-number-)| Directly changes the orders of the two series. |
| [swapSeries(number, number)](#swapSeries-number-number-)| Directly changes the orders of the two series. |
| [setSeriesNames(number, string, boolean)](#setSeriesNames-number-string-boolean-)| Sets the names of all the series in the chart. |
| [addR1C1(string, boolean)](#addR1C1-string-boolean-)| Adds the [Series](../series/) collection to a chart. |
| [add(string, boolean)](#add-string-boolean-)| Adds the [Series](../series/) collection to a chart. |
| [add(string, boolean, boolean)](#add-string-boolean-boolean-)| Adds the [Series](../series/) collection to a chart. |
| [clear()](#clear--)| Clears the collection |
| [changeColors(ChartColorPaletteType)](#changeColors-chartcolorpalettetype-)| Set Monochromatic Palette for chart series. |


### categoryData {#categoryData--}

Gets or sets the range of category Axis values. It can be a range of cells (such as "d1:e10") or a sequence of values (such as "{2,6,8,10}").

```javascript
categoryData : string;
```


### secondCategoryData {#secondCategoryData--}

Gets or sets the range of second category Axis values. It can be a range of cells (such as, "d1:e10"), or a sequence of values (such as,"{2,6,8,10}"). Only effects when some series were plotted on the second axis.

```javascript
secondCategoryData : string;
```


### isColorVaried {#isColorVaried--}

Represents if the color of points is varied.

```javascript
isColorVaried : boolean;
```


**Remarks**

Only works for pie chart or when there is only one series.

### get(number) {#get-number-}

Gets the [Series](../series/) element at the specified index.

```javascript
get(index: number) : Series;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### getSeriesByOrder(number) {#getSeriesByOrder-number-}

Gets the [Series](../series/) element by order.

```javascript
getSeriesByOrder(order: number) : Series;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| order | number | The order of series |

**Returns**

The element series

### removeAt(number) {#removeAt-number-}

Remove at a series at the specific index.

```javascript
removeAt(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

### changeSeriesOrder(number, number) {#changeSeriesOrder-number-number-}

Directly changes the orders of the two series.

```javascript
changeSeriesOrder(sourceIndex: number, destIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | number | The current index |
| destIndex | number | The dest index |

**Remarks**

NOTE: This method is now obsolete. Instead, please use SeriesCollection.SwapSeries method. This method will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### swapSeries(number, number) {#swapSeries-number-number-}

Directly changes the orders of the two series.

```javascript
swapSeries(sourceIndex: number, destIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | number | The current index |
| destIndex | number | The dest index |

### setSeriesNames(number, string, boolean) {#setSeriesNames-number-string-boolean-}

Sets the names of all the series in the chart.

```javascript
setSeriesNames(startIndex: number, area: string, isVertical: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number | The index of the first series which you want to set the name. |
| area | string | Specifies the area for the series name. |
| isVertical | boolean | >Specifies whether to plot the series from a range of cell values by row or by column. |

**Remarks**

br>If the start index is larger than the count of the serieses, it will return and do nothing.</br> <br>If set data on contiguous cells, use colon to separate them. For example, $C$2:$C$5.</br> <br>If set data on contiguous cells, use comma to separate them. For example, ($C$2,$D$5).</br

### addR1C1(string, boolean) {#addR1C1-string-boolean-}

Adds the [Series](../series/) collection to a chart.

```javascript
addR1C1(area: string, isVertical: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | string | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |

**Returns**

Return the first index of the added ASeries in the NSeries.

**Remarks**

br>If set data on contiguous cells, use colon to separate them. For example, R[1]C[1]:R[3]C[2].</br> <br>If set data on contiguous cells, use comma to separate them. For example,(R[1]C[1],R[3]C[2]).</br

### add(string, boolean) {#add-string-boolean-}

Adds the [Series](../series/) collection to a chart.

```javascript
add(dataArea: string, isVertical: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dataArea | string | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column.         /// If true, [Series](../series/) will be added column by column |

**Returns**

Return the first index of the added ASeries in the NSeries.

**Remarks**

br>If set data on contiguous cells, use colon to separate them.For example, $C$2:$C$5.</br> <br>If set data on non contiguous cells, use comma to separate them.For example: ($C$2,$D$5).</br> <br>This method only simply process <paramref name="dataArea"/> as data range. If you want to smartly check ChartCollection.Add() method. </br

### add(string, boolean, boolean) {#add-string-boolean-boolean-}

Adds the [Series](../series/) collection to a chart.

```javascript
add(area: string, isVertical: boolean, checkLabels: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| area | string | Specifies values from which to plot the data series |
| isVertical | boolean | Specifies whether to plot the series from a range of cell values by row or by column. |
| checkLabels | boolean | Indicates whether the range contains series's name |

**Returns**

Return the first index of the added ASeries in the NSeries.

**Remarks**

br>If set data on contiguous cells, use colon to separate them. For example, $C$2:$C$5.</br> <br>If set data on non contiguous cells, use comma to separate them. For example, ($C$2,$D$5).</br

### clear() {#clear--}

Clears the collection

```javascript
clear() : void;
```


### changeColors(ChartColorPaletteType) {#changeColors-chartcolorpalettetype-}

Set Monochromatic Palette for chart series.

```javascript
changeColors(type: ChartColorPaletteType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ChartColorPaletteType](../chartcolorpalettetype/) | The Monochromatic Type. |


