---
title: Trendline
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет линию тренда на диаграмме.
type: docs
weight: 980
url: /ru/net/aspose.cells.charts/trendline/
---
## Trendline class

Представляет линию тренда на диаграмме.

```csharp
public class Trendline : Line
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Backward](../../aspose.cells.charts/trendline/backward) { get; set; } | Возвращает или задает количество периодов (или единиц на точечной диаграмме), на которые линия тренда тянется назад. Количество периодов должно быть больше и равно нулю. Если тип диаграммы столбчатый, количество периодов должно быть от 0 до 0,5 |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength) { get; set; } | Указывает длину стрелки для начала строки. |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth) { get; set; } | Задает ширину стрелки для начала строки. |
| [BeginType](../../aspose.cells.drawing/line/begintype) { get; set; } | Указывает стрелку для начала строки. |
| [CapType](../../aspose.cells.drawing/line/captype) { get; set; } | Определяет конечные заглавные буквы. |
| [Color](../../aspose.cells.drawing/line/color) { get; set; } | ПредставляетColorлинии. |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype) { get; set; } | Задает тип составной линии |
| [DashType](../../aspose.cells.drawing/line/dashtype) { get; set; } | Указывает тип пунктирной линии |
| [DataLabels](../../aspose.cells.charts/trendline/datalabels) { get; } | Представляет объект DataLabels для указанного ASeries. |
| [DisplayEquation](../../aspose.cells.charts/trendline/displayequation) { get; set; } | Указывает, отображается ли на диаграмме уравнение для линии тренда (в той же метке данных, что и значение R-квадрата). Установка для этого свойства значения True автоматически включает метки данных. |
| [DisplayRSquared](../../aspose.cells.charts/trendline/displayrsquared) { get; set; } | Указывает, отображается ли на диаграмме значение R-квадрата линии тренда (в той же метке данных, что и уравнение). Установка для этого свойства значения True автоматически включает метки данных. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength) { get; set; } | Указывает длину стрелки для конца строки. |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth) { get; set; } | Задает ширину стрелки для конца строки. |
| [EndType](../../aspose.cells.drawing/line/endtype) { get; set; } | Указывает конец строки со стрелкой. |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype) { get; set; } | Получает или задает тип формата. |
| [Forward](../../aspose.cells.charts/trendline/forward) { get; set; } | Возвращает или задает количество периодов (или единиц на точечной диаграмме), на которое линия тренда продолжается вперед. Количество периодов должно быть больше и равно нулю. |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill) { get; } | Представляет градиентную заливку. |
| [Intercept](../../aspose.cells.charts/trendline/intercept) { get; set; } | Возвращает или задает точку, в которой линия тренда пересекает ось значений. |
| [IsAuto](../../aspose.cells.drawing/line/isauto) { get; set; } | Указывает, назначается ли этот стиль линии автоматически. |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor) { get; } | Указывает, назначается ли цвет линии автоматически. |
| [IsNameAuto](../../aspose.cells.charts/trendline/isnameauto) { get; set; } | Возвращает, если Microsoft Excel автоматически определяет имя линии тренда. |
| [IsVisible](../../aspose.cells.drawing/line/isvisible) { get; set; } | Указывает, видна ли линия. |
| [JoinType](../../aspose.cells.drawing/line/jointype) { get; set; } | Указывает соединительные заглавные буквы. |
| [LegendEntry](../../aspose.cells.charts/trendline/legendentry) { get; } | Получает запись легенды в соответствии с этой линией тренда |
| [Name](../../aspose.cells.charts/trendline/name) { get; set; } | Возвращает имя линии тренда. |
| [Order](../../aspose.cells.charts/trendline/order) { get; set; } | Возвращает или задает порядок линий тренда (целое число больше 1), если тип линии тренда полиномиальный. Порядок должен быть от 2 до 6. |
| [Period](../../aspose.cells.charts/trendline/period) { get; set; } | Возвращает или задает период для линии тренда скользящей средней. |
| [Style](../../aspose.cells.drawing/line/style) { get; set; } | Представляет стиль линии. |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor) { get; set; } | Получает и устанавливает цвет темы. |
| [Transparency](../../aspose.cells.drawing/line/transparency) { get; set; } | Возвращает или задает степень прозрачности линии как значение от 0,0 (непрозрачная) до 1,0 (прозрачная). |
| [Type](../../aspose.cells.charts/trendline/type) { get; } | Возвращает тип линии тренда. |
| [Weight](../../aspose.cells.drawing/line/weight) { get; set; } | Получает или задает[`WeightType`](../../aspose.cells.drawing/weighttype)линии. |
| [WeightPt](../../aspose.cells.drawing/line/weightpt) { get; set; } | Получает или задает вес линии в пунктах. |
| [WeightPx](../../aspose.cells.drawing/line/weightpx) { get; set; } | Получает или задает вес линии в единицах пикселей. |

### Примеры

```csharp

[C#]

  //Создание экземпляра рабочей книги object
Workbook workbook = new Workbook();
  //Добавление нового рабочего листа в Excel object
int sheetIndex = workbook.Worksheets.Add();
  //Получение ссылки на вновь добавленный рабочий лист путем передачи его листа index
Worksheet worksheet = workbook.Worksheets[sheetIndex];
  //Добавление значения выборки в "A1" cell
worksheet.Cells["A1"].PutValue(50);
//Добавление значения образца в "A2" cell
worksheet.Cells["A2"].PutValue(100);
  //Добавление значения образца в "A3" cell
worksheet.Cells["A3"].PutValue(150);
  //Добавление образца значения в "A4" cell
worksheet.Cells["A4"].PutValue(200);
  //Добавление образца значения в "B1" cell
worksheet.Cells["B1"].PutValue(60);
  //Добавление значения образца в "B2" cell
worksheet.Cells["B2"].PutValue(32);
  //Добавление значения образца в "B3" cell
worksheet.Cells["B3"].PutValue(50);
  //Добавление значения образца в "B4" cell
worksheet.Cells["B4"].PutValue(40);
  //Добавление образца значения в ячейку "C1" как категория data
worksheet.Cells["C1"].PutValue("Q1");
  //Добавление образца значения в ячейку "C2" как категория data
worksheet.Cells["C2"].PutValue("Q2");
  //Добавление значения образца в ячейку "C3" как категория data
worksheet.Cells["C3"].PutValue("Y1");
  //Добавление образца значения в ячейку "C4" как категория data
worksheet.Cells["C4"].PutValue("Y2");
  //Добавление диаграммы на лист
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
  //Доступ к экземпляру только что добавленного chart
Chart chart = worksheet.Charts[chartIndex];
  //Добавление NSeries (источника данных диаграммы) на диаграмму в диапазоне от ячейки "A1" до "B4"
chart.NSeries.Add("A1:B4", true);
  //Установка источника данных для данных категории NSeries
chart.NSeries.CategoryData = "C1:C4";
  //добавляем линейную линию тренда
int index = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
Trendline trendline = chart.NSeries[0].TrendLines[index];
  //Установка пользовательского имени линии тренда.
trendline.Name = "Linear";
  //Отображение уравнения на chart
trendline.DisplayEquation = true;
  //Отображение значения R-квадрата на chart
trendline.DisplayRSquared = true;
  //Сохранение файла Excel
workbook.Save("book1.xls");

[Visual Basic]

'Создание экземпляра рабочей книги object
Dim workbook As Workbook = New Workbook()
'Добавление нового рабочего листа в Excel object
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Получение ссылки на вновь добавленный рабочий лист путем передачи его листа index
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Добавление значения выборки в "A1" cell
worksheet.Cells("A1").PutValue(50)
'Добавление значения выборки в "A2" cell
worksheet.Cells("A2").PutValue(100)
'Добавление значения выборки в "A3" cell
worksheet.Cells("A3").PutValue(150)
'Добавление значения выборки в "A4" cell
worksheet.Cells("A4").PutValue(200)
'Добавление образца значения в "B1" cell
worksheet.Cells("B1").PutValue(60)
'Добавление образца значения в "B2" cell
worksheet.Cells("B2").PutValue(32)
'Добавление образца значения в "B3" cell
worksheet.Cells("B3").PutValue(50)
'Добавление образца значения в "B4" cell
worksheet.Cells("B4").PutValue(40)
'Добавление образца значения в ячейку "C1" как категория data
worksheet.Cells("C1").PutValue("Q1")
'Добавление образца значения в ячейку "C2" как категория data
worksheet.Cells("C2").PutValue("Q2")
'Добавление образца значения в ячейку "C3" как категория data
worksheet.Cells("C3").PutValue("Y1")
'Добавление образца значения в ячейку "C4" как категория data
worksheet.Cells("C4").PutValue("Y2")
'Добавление диаграммы на лист
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Доступ к экземпляру только что добавленного chart
Dim chart As Chart = worksheet.Charts(chartIndex)
'Добавление NSeries (источника данных диаграммы) на диаграмму в диапазоне от ячейки "A1" до "B4"
chart.NSeries.Add("A1:B4", True)
'Установка источника данных для данных категории NSeries
Chart.NSeries.CategoryData = "C1:C4"
'добавление линейной линии тренда
Dim index As Int32 = chart.NSeries(0).TrendLines.Add(TrendlineType.Linear)
Dim trendline As Trendline = chart.NSeries(0).TrendLines(index)
'Установка пользовательского имени линии тренда.
trendline.Name = "Linear"
'Отображение уравнения на chart
trendline.DisplayEquation = True
'Отображение значения R-квадрата на chart
trendline.DisplayRSquared = True
'Сохранение файла Excel
workbook.Save("book1.xls")
```

### Смотрите также

* class [Line](../../aspose.cells.drawing/line)
* пространство имен [Aspose.Cells.Charts](../../aspose.cells.charts)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
