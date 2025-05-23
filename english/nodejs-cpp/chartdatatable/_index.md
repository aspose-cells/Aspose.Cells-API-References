﻿---
title: ChartDataTable
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a chart data table.
type: docs
url: /nodejs-cpp/chartdatatable/
---

## ChartDataTable class

Represents a chart data table.

```javascript
class ChartDataTable;
```


### Example
```javascript
const { Workbook, ChartType, Color } = require("aspose.cells.node");

//Instantiating a Workbook object
var workbook = new Workbook();
//Obtaining the reference of the first worksheet
var worksheet = workbook.getWorksheets().get(0);
//Adding a sample value to "A1" cell
worksheet.getCells().get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.getCells().get("A2").putValue(100);
//Adding a sample value to "A3" cell
worksheet.getCells().get("A3").putValue(150);
//Adding a sample value to "B1" cell
worksheet.getCells().get("B1").putValue(60);
//Adding a sample value to "B2" cell
worksheet.getCells().get("B2").putValue(32);
//Adding a sample value to "B3" cell
worksheet.getCells().get("B3").putValue(50);
//Adding a chart to the worksheet
var chartIndex = worksheet.getCharts().add(ChartType.Column, 5, 0, 25, 10);
//Accessing the instance of the newly added chart
var chart = worksheet.getCharts().get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.getNSeries().add("A1:B3", true);
chart.setShowDataTable(true);
//Getting Chart Table
var chartTable = chart.getChartDataTable();
//Setting Chart Table Font Color
chartTable.getFont().setColor(Color.Red);
//Setting Legend Key Visibility
chartTable.setShowLegendKey(false);
//Saving the Excel file
workbook.save("output/ChartsChartDataTable.xls");
```
## Methods

| Method | Description |
| --- | --- |
| [getFont()](#getFont--)| Gets a [Font](../font/) object which represents the font setting of the specified chart data table. |
| [getAutoScaleFont()](#getAutoScaleFont--)| True if the text in the object changes font size when the object size changes. The default value is True. |
| [setAutoScaleFont(boolean)](#setAutoScaleFont-boolean-)| True if the text in the object changes font size when the object size changes. The default value is True. |
| [getBackgroundMode()](#getBackgroundMode--)| Gets and sets the display mode of the background |
| [setBackgroundMode(BackgroundMode)](#setBackgroundMode-backgroundmode-)| Gets and sets the display mode of the background |
| [getHasBorderHorizontal()](#getHasBorderHorizontal--)| True if the chart data table has horizontal cell borders |
| [setHasBorderHorizontal(boolean)](#setHasBorderHorizontal-boolean-)| True if the chart data table has horizontal cell borders |
| [getHasHorizontalBorder()](#getHasHorizontalBorder--)| True if the chart data table has horizontal cell borders |
| [setHasHorizontalBorder(boolean)](#setHasHorizontalBorder-boolean-)| True if the chart data table has horizontal cell borders |
| [getHasBorderVertical()](#getHasBorderVertical--)| True if the chart data table has vertical cell borders |
| [setHasBorderVertical(boolean)](#setHasBorderVertical-boolean-)| True if the chart data table has vertical cell borders |
| [getHasVerticalBorder()](#getHasVerticalBorder--)| True if the chart data table has vertical cell borders |
| [setHasVerticalBorder(boolean)](#setHasVerticalBorder-boolean-)| True if the chart data table has vertical cell borders |
| [getHasBorderOutline()](#getHasBorderOutline--)| True if the chart data table has outline borders |
| [setHasBorderOutline(boolean)](#setHasBorderOutline-boolean-)| True if the chart data table has outline borders |
| [getHasOutlineBorder()](#getHasOutlineBorder--)| True if the chart data table has outline borders |
| [setHasOutlineBorder(boolean)](#setHasOutlineBorder-boolean-)| True if the chart data table has outline borders |
| [getShowLegendKey()](#getShowLegendKey--)| True if the data label legend key is visible. |
| [setShowLegendKey(boolean)](#setShowLegendKey-boolean-)| True if the data label legend key is visible. |
| [getBorder()](#getBorder--)| Returns a Border object that represents the border of the object |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getFont() {#getFont--}

Gets a [Font](../font/) object which represents the font setting of the specified chart data table.

```javascript
getFont() : Font;
```


**Returns**

[Font](../font/)

### getAutoScaleFont() {#getAutoScaleFont--}

True if the text in the object changes font size when the object size changes. The default value is True.

```javascript
getAutoScaleFont() : boolean;
```


### setAutoScaleFont(boolean) {#setAutoScaleFont-boolean-}

True if the text in the object changes font size when the object size changes. The default value is True.

```javascript
setAutoScaleFont(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getBackgroundMode() {#getBackgroundMode--}

Gets and sets the display mode of the background

```javascript
getBackgroundMode() : BackgroundMode;
```


**Returns**

[BackgroundMode](../backgroundmode/)

### setBackgroundMode(BackgroundMode) {#setBackgroundMode-backgroundmode-}

Gets and sets the display mode of the background

```javascript
setBackgroundMode(value: BackgroundMode) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [BackgroundMode](../backgroundmode/) | The value to set. |

### getHasBorderHorizontal() {#getHasBorderHorizontal--}

True if the chart data table has horizontal cell borders

```javascript
getHasBorderHorizontal() : boolean;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasHorizontalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### setHasBorderHorizontal(boolean) {#setHasBorderHorizontal-boolean-}

True if the chart data table has horizontal cell borders

```javascript
setHasBorderHorizontal(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasHorizontalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### getHasHorizontalBorder() {#getHasHorizontalBorder--}

True if the chart data table has horizontal cell borders

```javascript
getHasHorizontalBorder() : boolean;
```


### setHasHorizontalBorder(boolean) {#setHasHorizontalBorder-boolean-}

True if the chart data table has horizontal cell borders

```javascript
setHasHorizontalBorder(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHasBorderVertical() {#getHasBorderVertical--}

True if the chart data table has vertical cell borders

```javascript
getHasBorderVertical() : boolean;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasVerticalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### setHasBorderVertical(boolean) {#setHasBorderVertical-boolean-}

True if the chart data table has vertical cell borders

```javascript
setHasBorderVertical(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasVerticalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### getHasVerticalBorder() {#getHasVerticalBorder--}

True if the chart data table has vertical cell borders

```javascript
getHasVerticalBorder() : boolean;
```


### setHasVerticalBorder(boolean) {#setHasVerticalBorder-boolean-}

True if the chart data table has vertical cell borders

```javascript
setHasVerticalBorder(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHasBorderOutline() {#getHasBorderOutline--}

True if the chart data table has outline borders

```javascript
getHasBorderOutline() : boolean;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasOutlineBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### setHasBorderOutline(boolean) {#setHasBorderOutline-boolean-}

True if the chart data table has outline borders

```javascript
setHasBorderOutline(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasOutlineBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### getHasOutlineBorder() {#getHasOutlineBorder--}

True if the chart data table has outline borders

```javascript
getHasOutlineBorder() : boolean;
```


### setHasOutlineBorder(boolean) {#setHasOutlineBorder-boolean-}

True if the chart data table has outline borders

```javascript
setHasOutlineBorder(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowLegendKey() {#getShowLegendKey--}

True if the data label legend key is visible.

```javascript
getShowLegendKey() : boolean;
```


### setShowLegendKey(boolean) {#setShowLegendKey-boolean-}

True if the data label legend key is visible.

```javascript
setShowLegendKey(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getBorder() {#getBorder--}

Returns a Border object that represents the border of the object

```javascript
getBorder() : Line;
```


**Returns**

[Line](../line/)

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



