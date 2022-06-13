---
title: Slicer
second_title: Справочник по Aspose.Cells для .NET API
description: краткое описание Slicer View
type: docs
weight: 5630
url: /ru/net/aspose.cells.slicers/slicer/
---
## Slicer class

краткое описание Slicer View

```csharp
public class Slicer
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [AlternativeText](../../aspose.cells.slicers/slicer/alternativetext) { get; set; } | Возвращает или задает описательную (альтернативную) текстовую строку объекта Slicer. |
| [Caption](../../aspose.cells.slicers/slicer/caption) { get; set; } | Возвращает или устанавливает заголовок указанного слайсера. |
| [CaptionVisible](../../aspose.cells.slicers/slicer/captionvisible) { get; set; } | Возвращает или устанавливает, виден ли заголовок, отображающий Caption слайсера значение по умолчанию - true |
| [ColumnWidth](../../aspose.cells.slicers/slicer/columnwidth) { get; set; } | Возвращает или задает ширину в пунктах каждого столбца в слайсере. |
| [ColumnWidthPixel](../../aspose.cells.slicers/slicer/columnwidthpixel) { get; set; } | Получает или задает ширину в пикселях для каждого столбца среза. |
| [Height](../../aspose.cells.slicers/slicer/height) { get; set; } | Возвращает или задает высоту указанного среза в пунктах. |
| [HeightPixel](../../aspose.cells.slicers/slicer/heightpixel) { get; set; } | Возвращает или задает высоту указанного среза в пикселях. |
| [IsLocked](../../aspose.cells.slicers/slicer/islocked) { get; set; } | Указывает, заблокирована ли форма среза. |
| [IsPrintable](../../aspose.cells.slicers/slicer/isprintable) { get; set; } | Указывает, доступен ли для печати объект среза. |
| [LeftPixel](../../aspose.cells.slicers/slicer/leftpixel) { get; set; } | Возвращает или задает горизонтальное смещение формы среза от его левого столбца в пикселях. |
| [LockedAspectRatio](../../aspose.cells.slicers/slicer/lockedaspectratio) { get; set; } | Указывает, блокируется ли соотношение сторон. |
| [LockedPosition](../../aspose.cells.slicers/slicer/lockedposition) { get; set; } | Указывает, можно ли перемещать указанный срез или изменять его размер с помощью пользовательского интерфейса. |
| [Name](../../aspose.cells.slicers/slicer/name) { get; set; } | Возвращает или задает имя указанного слайсера |
| [NumberOfColumns](../../aspose.cells.slicers/slicer/numberofcolumns) { get; set; } | Возвращает или задает количество столбцов в указанном срезе. |
| [Parent](../../aspose.cells.slicers/slicer/parent) { get; } | Возвращает объект Worksheet, представляющий лист, содержащий срез. Только для чтения. |
| [Placement](../../aspose.cells.slicers/slicer/placement) { get; set; } | Представляет способ прикрепления объекта рисования к ячейкам под ним. Свойство управляет размещением объекта на рабочем листе. |
| [RowHeight](../../aspose.cells.slicers/slicer/rowheight) { get; set; } | Возвращает или задает высоту в пунктах каждой строки в указанном срезе. |
| [RowHeightPixel](../../aspose.cells.slicers/slicer/rowheightpixel) { get; set; } | Возвращает или задает высоту в пикселях каждой строки в указанном срезе. |
| [SlicerCache](../../aspose.cells.slicers/slicer/slicercache) { get; } | Возвращает объект SlicerCache, связанный со слайсером. Только для чтения. |
| [StyleType](../../aspose.cells.slicers/slicer/styletype) { get; set; } | Укажите тип встроенного стиля слайсера Тип по умолчанию — SlicerStyleLight1 |
| [Title](../../aspose.cells.slicers/slicer/title) { get; set; } | Указывает заголовок текущего объекта Slicer. |
| [TopPixel](../../aspose.cells.slicers/slicer/toppixel) { get; set; } | Возвращает или задает вертикальное смещение формы среза от его верхней строки в пикселях. |
| [Width](../../aspose.cells.slicers/slicer/width) { get; set; } | Возвращает или задает ширину указанного среза в пунктах. |
| [WidthPixel](../../aspose.cells.slicers/slicer/widthpixel) { get; set; } | Возвращает или задает ширину указанного среза в пикселях. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddPivotConnection](../../aspose.cells.slicers/slicer/addpivotconnection)(PivotTable) | Добавляет соединение со сводной таблицей. |
| [Refresh](../../aspose.cells.slicers/slicer/refresh)() | Обновление слайсера. Тем временем обновление и расчет относительных сводных таблиц. |
| [RemovePivotConnection](../../aspose.cells.slicers/slicer/removepivotconnection)(PivotTable) | Удаляет подключение к сводной таблице. |

### Примеры

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
pivot.RefreshData();
pivot.CalculateData();

SlicerCollection slicers = sheet.Slicers;
int slicerIndex = slicers.Add(pivot, "E12", "fruit");
Slicer slicer = slicers[slicerIndex];
slicer.StyleType = SlicerStyleType.SlicerStyleLight2;

SlicerCacheItemCollection items = slicer.SlicerCache.SlicerCacheItems;
SlicerCacheItem item = items[0];
item.Selected = false;
  //делай свое дело
book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10
pivot.RefreshData()
pivot.CalculateData()

Dim slicers As SlicerCollection = sheet.Slicers
Dim slicerIndex As Int32 = slicers.Add(pivot, "E12", "fruit")
Dim slicer As Slicer = slicers(slicerIndex)
slicer.StyleType = SlicerStyleType.SlicerStyleLight2

Dim items As SlicerCacheItemCollection = slicer.SlicerCache.SlicerCacheItems
Dim item As SlicerCacheItem = items(0)
item.Selected = False

book.Save("out_vb.xlsx")
```

### Смотрите также

* пространство имен [Aspose.Cells.Slicers](../../aspose.cells.slicers)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
