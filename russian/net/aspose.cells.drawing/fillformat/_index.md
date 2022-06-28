---
title: FillFormat
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует объект представляющий форматирование заливки для фигуры.
type: docs
weight: 1970
url: /ru/net/aspose.cells.drawing/fillformat/
---
## FillFormat class

Инкапсулирует объект, представляющий форматирование заливки для фигуры.

```csharp
public class FillFormat
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [FillType](../../aspose.cells.drawing/fillformat/filltype) { get; set; } | Получает и устанавливает тип заливки |
| [GradientColor1](../../aspose.cells.drawing/fillformat/gradientcolor1) { get; } | Возвращает цвет градиента 1 для указанной заливки. |
| [GradientColor2](../../aspose.cells.drawing/fillformat/gradientcolor2) { get; } | Возвращает цвет градиента 2 для указанной заливки. |
| [GradientColorType](../../aspose.cells.drawing/fillformat/gradientcolortype) { get; } | Возвращает тип цвета градиента для указанной заливки. |
| [GradientDegree](../../aspose.cells.drawing/fillformat/gradientdegree) { get; } | Возвращает степень градиента для указанной заливки. Применяется только для Excel 2007. |
| [GradientFill](../../aspose.cells.drawing/fillformat/gradientfill) { get; } | Получает[`GradientFill`](./gradientfill)объект. |
| [GradientStyle](../../aspose.cells.drawing/fillformat/gradientstyle) { get; } | Возвращает стиль градиента для указанной заливки. |
| [GradientVariant](../../aspose.cells.drawing/fillformat/gradientvariant) { get; } | Возвращает вариант градиента для указанной заливки. Применяется только для Excel 2007. |
| [ImageData](../../aspose.cells.drawing/fillformat/imagedata) { get; set; } | Получает и устанавливает данные изображения изображения. |
| [Pattern](../../aspose.cells.drawing/fillformat/pattern) { get; set; } | Представляет шаблон отображения области. |
| [PatternFill](../../aspose.cells.drawing/fillformat/patternfill) { get; } | Получает[`PatternFill`](./patternfill)объект. |
| [PictureFormatType](../../aspose.cells.drawing/fillformat/pictureformattype) { get; set; } | Получает и задает тип формата изображения. |
| [PresetColor](../../aspose.cells.drawing/fillformat/presetcolor) { get; } | Возвращает заданный цвет градиента для указанной заливки. |
| [Scale](../../aspose.cells.drawing/fillformat/scale) { get; set; } | Получает и задает масштаб формата изображения. |
| [SolidFill](../../aspose.cells.drawing/fillformat/solidfill) { get; } | Получает объект[`SolidFill`](./solidfill). |
| [Texture](../../aspose.cells.drawing/fillformat/texture) { get; set; } | Представляет тип текстуры для указанной заливки. |
| [TextureFill](../../aspose.cells.drawing/fillformat/texturefill) { get; } | Получает объект[`TextureFill`](./texturefill). |
| [Transparency](../../aspose.cells.drawing/fillformat/transparency) { get; set; } | Возвращает или задает степень прозрачности области в виде значения от 0,0 (непрозрачная) до 1,0 (прозрачная). |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fillformat/equals)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/fillformat/gethashcode)() | Получает хэш-код. |
| [SetOneColorGradient](../../aspose.cells.drawing/fillformat/setonecolorgradient)(Color, double, GradientStyleType, int) | Устанавливает для указанной заливки одноцветный градиент. Применяется только для Excel 2007. |
| [SetPresetColorGradient](../../aspose.cells.drawing/fillformat/setpresetcolorgradient)(GradientPresetType, GradientStyleType, int) | Устанавливает для указанной заливки заданный градиент цвета. Применяется только для Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Устанавливает для указанной заливки двухцветный градиент. Применяется только для Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/fillformat/settwocolorgradient#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Устанавливает для указанной заливки двухцветный градиент. Применяется только для Excel 2007. |

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
int seriesIndex = chart.NSeries.Add("A1:B4", true);
  //Установка источника данных для данных категории NSeries
chart.NSeries.CategoryData = "C1:C4";
//Заливка области 2-го NSeries градиентом
chart.NSeries[seriesIndex].Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1);

[Visual Basic]

Создание экземпляра рабочей книги object
Dim workbook As Workbook = New Workbook()
'Добавление нового рабочего листа в Excel object
Dim sheetIndex As Int32 = workbook.Worksheets.Add()
'Получение ссылки на недавно добавленный рабочий лист путем передачи его индекса листа
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Добавление значения выборки в "A1" cell
worksheet.Cells("A1").PutValue(50)
'Добавление значения выборки в "A2" cell
worksheet.Cells("A2").PutValue(100)
'Добавление значения выборки в "A3" cell
worksheet.Cells("A3").PutValue(150)
'Добавление значения выборки в "A4" cell
worksheet.Cells("A4").PutValue(200)
'Добавление значения выборки в "B1" cell
worksheet.Cells("B1").PutValue(60)
'Добавление значения выборки в "B2" cell
worksheet.Cells("B2").PutValue(32)
'Добавление значения выборки в "B3" cell
worksheet.Cells("B3").PutValue(50)
'Добавление значения выборки в "B4" cell
worksheet.Cells("B4").PutValue(40)
'Добавление образца значения в ячейку "C1" как категория data
worksheet.Cells("C1").PutValue("Q1")
'Добавление образца значения в ячейку "C2" как категория data
worksheet.Cells("C2").PutValue("Q2")
'Добавление образца значения в ячейку "C3" как категория data
worksheet.Cells("C3").PutValue("Y1")
'Добавление образца значения в ячейку "C4" как категория data
worksheet.Cells("C4").PutValue("Y2")
'Добавление диаграммы на рабочий лист
Dim chartIndex As Int32 = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Доступ к экземпляру вновь добавленной диаграммы
Dim chart As Chart = worksheet.Charts(chartIndex)
'Добавление NSeries (источника данных диаграммы) на диаграмму в диапазоне от ячейки "A1" до "B4"
Dim seriesIndex As Int32 = chart.NSeries.Add("A1:B4", True)
'Установка источника данных для данных категории NSeries
chart.NSeries.CategoryData = "C1:C4"
'Заливка области 2-го NSeries градиентом
chart.NSeries(seriesIndex).Area.FillFormat.SetOneColorGradient(Color.Lime, 1, GradientStyleType.Horizontal, 1)
```

### Смотрите также

* пространство имен [Aspose.Cells.Drawing](../../aspose.cells.drawing)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
