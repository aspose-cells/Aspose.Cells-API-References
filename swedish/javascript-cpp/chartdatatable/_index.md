---
title: ChartDataTable
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents a chart data table.
type: docs
url: /sv/javascript-cpp/chartdatatable/
---

## ChartDataTable class

Represents a chart data table.

```javascript
class ChartDataTable;
```


### Example
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//Instansiering av ett Workbook-objekt
var workbook = new Workbook();
//Hämtar referensen till det första kalkylbladet
var worksheet = workbook.worksheets.get(0);
//Lägger till ett exempelvärde i cellen "A1"
worksheet.cells.get("A1").putValue(50);
//Lägger till ett exempelvärde i cellen "A2"
worksheet.cells.get("A2").putValue(100);
//Lägger till ett exempelvärde i cellen "A3"
worksheet.cells.get("A3").putValue(150);
//Lägger till ett exempelvärde i cellen "B1"
worksheet.cells.get("B1").putValue(60);
//Lägger till ett exempelvärde i cellen "B2"
worksheet.cells.get("B2").putValue(32);
//Lägger till ett exempelvärde i cellen "B3"
worksheet.cells.get("B3").putValue(50);
//Lägger till ett diagram i kalkylbladet
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 25, 10);
//Åtkomst till instansen av det nyss tillagda diagrammet
var chart = worksheet.charts.get(chartIndex);
//Lägger till NSeries (diagramdatakälla) i diagrammet från cell "A1" till "B3"
chart.nSeries.add("A1:B3", true);
chart.showDataTable = true;
//Hämtar diagramtabell
var chartTable = chart.getChartDataTable();
//Ställer in diagramtabellens teckensnittsfärg
chartTable.font.color = Color.Red;
//Ställer in legendnyckelns synlighet
chartTable.showLegendKey = false;
//Sparar Excel-filen
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [font](#font--)| Font | Readonly. Gets a [Font](../font/) object which represents the font setting of the specified chart data table. |
| [autoScaleFont](#autoScaleFont--)| boolean | True if the text in the object changes font size when the object size changes. The default value is True. |
| [backgroundMode](#backgroundMode--)| BackgroundMode | Gets and sets the display mode of the background |
| [hasBorderHorizontal](#hasBorderHorizontal--)| boolean | True if the chart data table has horizontal cell borders |
| [hasHorizontalBorder](#hasHorizontalBorder--)| boolean | True if the chart data table has horizontal cell borders |
| [hasBorderVertical](#hasBorderVertical--)| boolean | True if the chart data table has vertical cell borders |
| [hasVerticalBorder](#hasVerticalBorder--)| boolean | True if the chart data table has vertical cell borders |
| [hasBorderOutline](#hasBorderOutline--)| boolean | True if the chart data table has outline borders |
| [hasOutlineBorder](#hasOutlineBorder--)| boolean | True if the chart data table has outline borders |
| [showLegendKey](#showLegendKey--)| boolean | True if the data label legend key is visible. |
| [border](#border--)| Line | Readonly. Returns a Border object that represents the border of the object |


### font {#font--}

Readonly. Gets a [Font](../font/) object which represents the font setting of the specified chart data table.

```javascript
font : Font;
```


### autoScaleFont {#autoScaleFont--}

True if the text in the object changes font size when the object size changes. The default value is True.

```javascript
autoScaleFont : boolean;
```


### backgroundMode {#backgroundMode--}

Gets and sets the display mode of the background

```javascript
backgroundMode : BackgroundMode;
```


### hasBorderHorizontal {#hasBorderHorizontal--}

True if the chart data table has horizontal cell borders

```javascript
hasBorderHorizontal : boolean;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasHorizontalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### hasHorizontalBorder {#hasHorizontalBorder--}

True if the chart data table has horizontal cell borders

```javascript
hasHorizontalBorder : boolean;
```


### hasBorderVertical {#hasBorderVertical--}

True if the chart data table has vertical cell borders

```javascript
hasBorderVertical : boolean;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasVerticalBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### hasVerticalBorder {#hasVerticalBorder--}

True if the chart data table has vertical cell borders

```javascript
hasVerticalBorder : boolean;
```


### hasBorderOutline {#hasBorderOutline--}

True if the chart data table has outline borders

```javascript
hasBorderOutline : boolean;
```


**Remarks**

NOTE: This property is now obsolete. Instead, please use ChartDataTable.HasOutlineBorder property. This property will be removed 12 months later since June 2024. Aspose apologizes for any inconvenience you may have experienced.

### hasOutlineBorder {#hasOutlineBorder--}

True if the chart data table has outline borders

```javascript
hasOutlineBorder : boolean;
```


### showLegendKey {#showLegendKey--}

True if the data label legend key is visible.

```javascript
showLegendKey : boolean;
```


### border {#border--}

Readonly. Returns a Border object that represents the border of the object

```javascript
border : Line;
```



