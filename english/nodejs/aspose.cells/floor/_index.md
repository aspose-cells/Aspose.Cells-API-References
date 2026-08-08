---
title: "Floor"
linktitle: "Floor"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates the object that represents the floor of a 3-D chart."
type: docs
weight: 1510
url: /nodejs/aspose.cells/floor/
---

## Floor class

Encapsulates the object that represents the floor of a 3-D chart.

## Methods

| Name | Description |
| --- | --- |
| [getBackgroundColor()](#getbackgroundcolor) | Gets or sets the background com.aspose.cells.Color of the Area. |
| [getBorder()](#getborder) | Gets or sets the border Line. |
| [getFillFormat()](#getfillformat) | Represents a FillFormat object that contains fill formatting properties for the specified chart or shape. |
| [getForegroundColor()](#getforegroundcolor) | Gets or sets the foreground com.aspose.cells.Color. |
| [getFormatting()](#getformatting) | Represents the formatting of the area. The value of the property is FormattingType integer constant. |
| [getInvertIfNegative()](#getinvertifnegative) | If the property is true and the value of chart point is a negative number, the foreground color and background color wil |
| [getTransparency()](#gettransparency) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setBackgroundColor()](#setbackgroundcolor) | Gets or sets the background com.aspose.cells.Color of the Area. |
| [setBorder()](#setborder) | Gets or sets the border Line. |
| [setForegroundColor()](#setforegroundcolor) | Gets or sets the foreground com.aspose.cells.Color. |
| [setFormatting()](#setformatting) | Represents the formatting of the area. The value of the property is FormattingType integer constant. |
| [setInvertIfNegative()](#setinvertifnegative) | If the property is true and the value of chart point is a negative number, the foreground color and background color wil |
| [setTransparency()](#settransparency) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |

### getBackgroundColor() {#getbackgroundcolor}

Gets or sets the background com.aspose.cells.Color of the Area.

### getBorder() {#getborder}

Gets or sets the border Line.

### getFillFormat() {#getfillformat}

Represents a FillFormat object that contains fill formatting properties for the specified chart or shape.

### getForegroundColor() {#getforegroundcolor}

Gets or sets the foreground com.aspose.cells.Color.

### getFormatting() {#getformatting}

Represents the formatting of the area. The value of the property is FormattingType integer constant.

### getInvertIfNegative() {#getinvertifnegative}

If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

**Example:**

```js
//Instantiating a Workbook object
var workbook = new aspose.cells.Workbook();
//Adding a new worksheet to the Workbook object
var sheetIndex = workbook.getWorksheets().add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.getWorksheets().get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.getCells().get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.getCells().get("A2").putValue(-100);
//Adding a sample value to "A3" cell
worksheet.getCells().get("A3").putValue(150);
//Adding a chart to the worksheet
var chartIndex = worksheet.getCharts().add(aspose.cells.ChartType.COLUMN, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.getCharts().get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "A3"
chart.getNSeries().add("A1:A3", true);
chart.getNSeries().get(0).getArea().setInvertIfNegative(true);
//Setting the foreground color of the 1st NSeries area
chart.getNSeries().get(0).getArea().setForegroundColor(aspose.cells.Color.getRed());
//Setting the background color of the 1st NSeries area.
//The displayed area color of second chart point will be the background color.
chart.getNSeries().get(0).getArea().setBackgroundColor(aspose.cells.Color.getYellow());
//Saving the Excel file
workbook.save("C:\\book1.xls");
```

### getTransparency() {#gettransparency}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

### setBackgroundColor() {#setbackgroundcolor}

Gets or sets the background com.aspose.cells.Color of the Area.

### setBorder() {#setborder}

Gets or sets the border Line.

### setForegroundColor() {#setforegroundcolor}

Gets or sets the foreground com.aspose.cells.Color.

### setFormatting() {#setformatting}

Represents the formatting of the area. The value of the property is FormattingType integer constant.

### setInvertIfNegative() {#setinvertifnegative}

If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

**Example:**

```js
//Instantiating a Workbook object
var workbook = new aspose.cells.Workbook();
//Adding a new worksheet to the Workbook object
var sheetIndex = workbook.getWorksheets().add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.getWorksheets().get(sheetIndex);
//Adding a sample value to "A1" cell
worksheet.getCells().get("A1").putValue(50);
//Adding a sample value to "A2" cell
worksheet.getCells().get("A2").putValue(-100);
//Adding a sample value to "A3" cell
worksheet.getCells().get("A3").putValue(150);
//Adding a chart to the worksheet
var chartIndex = worksheet.getCharts().add(aspose.cells.ChartType.COLUMN, 5, 0, 15, 5);
//Accessing the instance of the newly added chart
var chart = worksheet.getCharts().get(chartIndex);
//Adding NSeries (chart data source) to the chart ranging from "A1" cell to "A3"
chart.getNSeries().add("A1:A3", true);
chart.getNSeries().get(0).getArea().setInvertIfNegative(true);
//Setting the foreground color of the 1st NSeries area
chart.getNSeries().get(0).getArea().setForegroundColor(aspose.cells.Color.getRed());
//Setting the background color of the 1st NSeries area.
//The displayed area color of second chart point will be the background color.
chart.getNSeries().get(0).getArea().setBackgroundColor(aspose.cells.Color.getYellow());
//Saving the Excel file
workbook.save("C:\\book1.xls");
```

### setTransparency() {#settransparency}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
