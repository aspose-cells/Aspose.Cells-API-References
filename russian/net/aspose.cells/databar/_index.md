---
title: DataBar
second_title: Справочник по Aspose.Cells для .NET API
description: Опишите правило условного форматирования DataBar. Это правило условного форматирования отображает градуированную панель данных в диапазоне ячеек.
type: docs
weight: 1240
url: /ru/net/aspose.cells/databar/
---
## DataBar class

Опишите правило условного форматирования DataBar. Это правило условного форматирования отображает градуированную панель данных в диапазоне ячеек.

```csharp
public class DataBar
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [AxisColor](../../aspose.cells/databar/axiscolor) { get; set; } | Получает цвет оси для ячеек с условным форматированием в виде гистограмм. |
| [AxisPosition](../../aspose.cells/databar/axisposition) { get; set; } | Получает или задает положение оси гистограмм, заданное правилом условного форматирования. |
| [BarBorder](../../aspose.cells/databar/barborder) { get; } | Получает объект, указывающий границу гистограммы. |
| [BarFillType](../../aspose.cells/databar/barfilltype) { get; set; } | Получает или задает способ заполнения панели данных цветом. |
| [Color](../../aspose.cells/databar/color) { get; set; } | Получить или установить цвет этого DataBar. |
| [Direction](../../aspose.cells/databar/direction) { get; set; } | Получает или задает направление отображения панели данных. |
| [MaxCfvo](../../aspose.cells/databar/maxcfvo) { get; } | Получите или установите объект максимального значения этого DataBar. Невозможно установить значение null или CFValueObject с типом FormatConditionValueType.Min. |
| [MaxLength](../../aspose.cells/databar/maxlength) { get; set; } | Представляет максимальную длину строки данных. |
| [MinCfvo](../../aspose.cells/databar/mincfvo) { get; } | Получить или установить объект минимального значения этого DataBar. Невозможно установить значение null или CFValueObject с типом FormatConditionValueType.Max. |
| [MinLength](../../aspose.cells/databar/minlength) { get; set; } | Представляет минимальную длину строки данных. |
| [NegativeBarFormat](../../aspose.cells/databar/negativebarformat) { get; } | Получает объект NegativeBarFormat, связанный с правилом условного форматирования гистограммы. |
| [ShowValue](../../aspose.cells/databar/showvalue) { get; set; } | Получите или установите флаг, указывающий, следует ли отображать значения ячеек, к которым применяется эта панель данных. Значение по умолчанию — true. |

## Методы

| Имя | Описание |
| --- | --- |
| [ToImage](../../aspose.cells/databar/toimage)(Cell, ImageOrPrintOptions) | Отобразить панель данных в ячейке в массив байтов изображения. |

### Примеры

```csharp

[C#]

  //Создание экземпляра рабочей книги object
Workbook workbook = new Workbook();

Worksheet sheet = workbook.Worksheets[0];

  //Добавляет пустое условное форматирование
int index = sheet.ConditionalFormattings.Add();

FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

  //Устанавливает диапазон условного формата.
CellArea ca = new CellArea();

ca.StartRow = 0;

ca.EndRow = 2;

ca.StartColumn = 0;

ca.EndColumn = 0;

fcs.AddArea(ca);

  //Добавляет условие.
int idx = fcs.AddCondition(FormatConditionType.DataBar);

fcs.AddArea(ca);

FormatCondition cond = fcs[idx];

  //Получить панель данных
DataBar dataBar = cond.DataBar;

dataBar.Color = Color.Orange;

  //Установить свойства панели данных
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;

dataBar.MinCfvo.Value = 30;

dataBar.ShowValue = false;

dataBar.BarBorder.Type = DataBarBorderType.Solid;

dataBar.BarBorder.Color = Color.Plum;

 dataBar.BarFillType = DataBarFillType.Solid;
  
 dataBar.AxisColor = Color.Red;
 
 dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
 
 dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
 
 dataBar.NegativeBarFormat.Color = Color.White;
 
 dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
 
 dataBar.NegativeBarFormat.BorderColor = Color.Yellow;
 
  //Поместите значения ячеек
Aspose.Cells.Cell cell1 = sheet.Cells["A1"];

cell1.PutValue(10);

Aspose.Cells.Cell cell2 = sheet.Cells["A2"];

cell2.PutValue(120);

Aspose.Cells.Cell cell3 = sheet.Cells["A3"];

cell3.PutValue(260);

  //Сохранение файла Excel
workbook.Save("book1.xlsx");

[VB.NET]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()

Dim sheet As Worksheet = workbook.Worksheets(0)

'Adds an empty conditional formatting
Dim index As Integer = sheet.ConditionalFormattings.Add()

Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)

'Sets the conditional format range.
Dim ca As New CellArea()

ca.StartRow = 0

ca.EndRow = 2

ca.StartColumn = 0

ca.EndColumn = 0

fcs.AddArea(ca)

'Adds condition.
Dim idx As Integer = fcs.AddCondition(FormatConditionType.DataBar)

fcs.AddArea(ca)

Dim cond As FormatCondition = fcs(idx)

'Get Databar
Dim dataBar As DataBar = cond.DataBar

dataBar.Color = Color.Orange

'Set Databar properties
dataBar.MinCfvo.Type = FormatConditionValueType.Percentile

dataBar.MinCfvo.Value = 30

dataBar.ShowValue = False

dataBar.BarBorder.Type = DataBarBorderType.Solid

dataBar.BarBorder.Color = Color.Plum

 dataBar.BarFillType = DataBarFillType.Solid
  
 dataBar.AxisColor = Color.Red
 
 dataBar.AxisPosition = DataBarAxisPosition.Midpoint
 
 dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color
 
 dataBar.NegativeBarFormat.Color = Color.White
 
 dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color
 
 dataBar.NegativeBarFormat.BorderColor = Color.Yellow

'Put Cell Values
Dim cell1 As Aspose.Cells.Cell = sheet.Cells("A1")

cell1.PutValue(10)

Dim cell2 As Aspose.Cells.Cell = sheet.Cells("A2")

cell2.PutValue(120)

Dim cell3 As Aspose.Cells.Cell = sheet.Cells("A3")

cell3.PutValue(260)

'Saving the Excel file
workbook.Save("book1.xlsx")

```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
