---
title: ChartArea
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует объект представляющий область диаграммы на листе.
type: docs
weight: 440
url: /ru/net/aspose.cells.charts/chartarea/
---
## ChartArea class

Инкапсулирует объект, представляющий область диаграммы на листе.

```csharp
public class ChartArea : ChartFrame
```

## Характеристики

| Имя | Описание |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area) { get; } | Получает[`область`](../chartframe/area) . |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont) { get; set; } | Истинно, если текст в объекте меняет размер шрифта при изменении размера объекта. Значение по умолчанию верно. |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode) { get; set; } | Получает и устанавливает режим отображения background |
| virtual [Border](../../aspose.cells.charts/chartframe/border) { get; } | Получает[`граница`](../../aspose.cells.drawing/line) . |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight) { get; } | Представляет высоту позиции по умолчанию |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth) { get; } | Представляет ширину позиции по умолчанию |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx) { get; } | Представляет x позиции по умолчанию |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty) { get; } | Представляет y позиции по умолчанию |
| override [Font](../../aspose.cells.charts/chartarea/font) { get; } | Получает[`Font`](./font) объект указанного объекта диаграммы. |
| override [Height](../../aspose.cells.charts/chartarea/height) { get; set; } | Получает или задает вертикальное смещение от нижнего правого углового ряда. |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize) { get; set; } | Указывает, имеет ли рамка диаграммы автоматический размер. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset) { get; } | Указывает, установлены ли позиции по умолчанию (DefaultX, DefaultY, DefaultWidth и DefaultHeight). |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode) { get; set; } | Указывает, включает ли размер области графика деления и метки осей. False указывает, что размер должен определять размер области графика, деления и метки осей. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow) { get; set; } | Истинно, если у кадра есть тень. |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties) { get; } | Получает[`ShapeProperties`](../chartframe/shapeproperties) объект. |
| override [Width](../../aspose.cells.charts/chartarea/width) { get; set; } | Получает или задает смещение по горизонтали от нижнего правого углового столбца. |
| override [X](../../aspose.cells.charts/chartarea/x) { get; set; } | Получает или получает горизонтальное смещение от верхнего левого углового столбца. |
| override [Y](../../aspose.cells.charts/chartarea/y) { get; set; } | Получает или получает вертикальное смещение от строки верхнего левого угла. |

## Методы

| Имя | Описание |
| --- | --- |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto)() | Установить положение кадра на auto |

### Примеры

```csharp

[C#]

//Создание экземпляра объекта Workbook
Workbook workbook = new Workbook();

//Получение ссылки на первый рабочий лист
Worksheet worksheet = workbook.Worksheets[0];

//Добавление пробного значения в ячейку "A1"
worksheet.Cells["A1"].PutValue(50);

//Добавление образца значения в ячейку "A2"
worksheet.Cells["A2"].PutValue(100);

//Добавление образца значения в ячейку "A3"
worksheet.Cells["A3"].PutValue(150);

//Добавление образца значения в ячейку "B1"
worksheet.Cells["B1"].PutValue(60);

//Добавление образца значения в ячейку "B2"
worksheet.Cells["B2"].PutValue(32);

//Добавление образца значения в ячейку "B3"
worksheet.Cells["B3"].PutValue(50);

//Добавляем диаграмму на рабочий лист
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);

//Доступ к экземпляру только что добавленного графика
Chart chart = worksheet.Charts[chartIndex];

//Добавление NSeries (источника данных диаграммы) на диаграмму в диапазоне от ячейки "A1" до "B3"
chart.NSeries.Add("A1:B3", true);

//Получение области графика
ChartArea chartArea = chart.ChartArea;

//Установка цвета переднего плана области графика
chartArea.Area.ForegroundColor = Color.Yellow;

//Установка тени области графика
chartArea.Shadow = true;

//Сохранение файла Excel
workbook.Save("book1.xls");

[VB.NET]

'Создание экземпляра объекта Workbook
Dim workbook As Workbook = New Workbook()

'Получение ссылки на первый рабочий лист
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)

'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)

'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)

'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)

'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)

'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)

'Добавление диаграммы на рабочий лист
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)

'Доступ к экземпляру вновь добавленной диаграммы
Dim chart As Chart = worksheet.Charts(chartIndex)

'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.NSeries.Add("A1:B3", True)

'Получение области диаграммы
Dim chartArea As ChartArea = chart.ChartArea

'Установка цвета переднего плана области диаграммы
chartArea.Area.ForegroundColor = Color.Yellow

'Настройка тени области диаграммы
chartArea.Shadow = True

'Сохранение файла Excel
workbook.Save("book1.xls")
```

### Смотрите также

* class [ChartFrame](../chartframe)
* пространство имен [Aspose.Cells.Charts](../../aspose.cells.charts)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
