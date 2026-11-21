---
title: Area
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates the object that represents an area format.
type: docs
url: /ru/javascript-cpp/area/
---

## Area class

Encapsulates the object that represents an area format.

```javascript
class Area;
```


### Example
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//Создание объекта Workbook
var workbook = new Workbook();
//Добавление нового листа в объект Workbook
var sheetIndex = workbook.worksheets.add();
//Получение ссылки на только что добавленный лист, передавая его индекс листа
var worksheet = workbook.worksheets.get(sheetIndex);
//Добавление примерного значения в ячейку "A1"
worksheet.cells.get("A1").putValue(50);
//Добавление примерного значения в ячейку "A2"
worksheet.cells.get("A2").putValue(100);
//Добавление примерного значения в ячейку "A3"
worksheet.cells.get("A3").putValue(150);
//Добавление примерного значения в ячейку "B1"
worksheet.cells.get("B1").putValue(60);
//Добавление примерного значения в ячейку "B2"
worksheet.cells.get("B2").putValue(32);
//Добавление примерного значения в ячейку "B3"
worksheet.cells.get("B3").putValue(50);
//Добавление диаграммы на лист
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Получение экземпляра только что добавленной диаграммы
var chart = worksheet.charts.get(chartIndex);
//Добавление NSeries (источник данных диаграммы) к диаграмме в диапазоне от ячейки "A1" до "B3"
chart.nSeries.add("A1:B3", true);
//Установка цвета переднего плана области построения
chart.plotArea.getArea().foregroundColor = Color.Blue;
//Установка цвета переднего плана области диаграммы
chart.chartArea.getArea().foregroundColor = Color.Yellow;
//Установка цвета переднего плана области 1-го NSeries
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Установка цвета переднего плана области 1-го пункта NSeries
chart.nSeries.get(0).points.get(0).area.foregroundColor = Color.Cyan;
//Сохранение файла Excel
var uint8Array = workbook.save(SaveFormat.Excel97To2003);
```
## Properties

| Property | Type | Description |
| --- | --- | --- |
| [backgroundColor](#backgroundColor--)| Color | Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [foregroundColor](#foregroundColor--)| Color | Gets or sets the foreground [Color](../color/). |
| [formatting](#formatting--)| FormattingType | Represents the formatting of the area. |
| [invertIfNegative](#invertIfNegative--)| boolean | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [fillFormat](#fillFormat--)| FillFormat | Readonly. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |


### backgroundColor {#backgroundColor--}

Gets or sets the background [Color](../color/) of the [Area](../area/).

```javascript
backgroundColor : Color;
```


### foregroundColor {#foregroundColor--}

Gets or sets the foreground [Color](../color/).

```javascript
foregroundColor : Color;
```


### formatting {#formatting--}

Represents the formatting of the area.

```javascript
formatting : FormattingType;
```


### invertIfNegative {#invertIfNegative--}

If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.

```javascript
invertIfNegative : boolean;
```


**Example**
```javascript
const { Workbook, ChartType, Color, SaveFormat } = AsposeCells;

//Создание объекта Workbook
var workbook = new Workbook();
//Добавление нового листа в объект Workbook
var sheetIndex = workbook.worksheets.add();
//Получение ссылки на только что добавленный лист, передавая его индекс листа
var worksheet = workbook.worksheets.get(sheetIndex);
//Добавление примерного значения в ячейку "A1"
worksheet.cells.get("A1").putValue(50);
//Добавление примерного значения в ячейку "A2"
worksheet.cells.get("A2").putValue(-100);
//Добавление примерного значения в ячейку "A3"
worksheet.cells.get("A3").putValue(150);
//Добавление диаграммы на лист
var chartIndex = worksheet.charts.add(ChartType.Column, 5, 0, 15, 5);
//Получение экземпляра только что добавленной диаграммы
var chart = worksheet.charts.get(chartIndex);
//Добавление NSeries (источник данных диаграммы) к диаграмме, охватывающей ячейки от "A1" до "A3"
chart.nSeries.add("A1:A3", true);
chart.nSeries.get(0).area.invertIfNegative = true;
//Установка цвета переднего плана области 1-го NSeries
chart.nSeries.get(0).area.foregroundColor = Color.Red;
//Установка цвета фона области 1-го NSeries.
//Отображаемый цвет области второй точки диаграммы будет цветом фона.
chart.nSeries.get(0).area.backgroundColor = Color.Yellow;
//Сохранение файла Excel
var uint8Array = workbook.save(SaveFormat.Excel97To2003);
```

### fillFormat {#fillFormat--}

Readonly. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape.

```javascript
fillFormat : FillFormat;
```


### transparency {#transparency--}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
transparency : number;
```



