---
title: Slicer
second_title: Aspose.Cells for .NET API Reference
description: 
type: docs
weight: 5600
url: /net/aspose.cells.slicers/slicer/
---
## Slicer class

summary description of Slicer View

```csharp
public class Slicer
```

## Properties

| Name | Description |
| --- | --- |
| [AlternativeText](alternativetext) { get; set; } | Returns or sets the descriptive (alternative) text string of the Slicer object. |
| [Caption](caption) { get; set; } | Returns or sets the caption of the specified slicer. |
| [CaptionVisible](captionvisible) { get; set; } | Returns or sets whether the header that displays the slicer Caption is visible the default value is true |
| [ColumnWidth](columnwidth) { get; set; } | Returns or sets the width, in points, of each column in the slicer. |
| [ColumnWidthPixel](columnwidthpixel) { get; set; } | Gets or sets the width in unit of pixels for each column of the slicer. |
| [Height](height) { get; set; } | Returns or sets the height of the specified slicer, in points. |
| [HeightPixel](heightpixel) { get; set; } | Returns or sets the height of the specified slicer, in pixels. |
| [IsLocked](islocked) { get; set; } | Indicates whether the slicer shape is locked. |
| [IsPrintable](isprintable) { get; set; } | Indicates whether the slicer object is printable. |
| [LeftPixel](leftpixel) { get; set; } | Returns or sets the horizontal offset of slicer shape from its left column, in pixels. |
| [LockedAspectRatio](lockedaspectratio) { get; set; } | Indicates whether locking aspect ratio. |
| [LockedPosition](lockedposition) { get; set; } | Indicates whether the specified slicer can be moved or resized by using the user interface. |
| [Name](name) { get; set; } | Returns or sets the name of the specified slicer |
| [NumberOfColumns](numberofcolumns) { get; set; } | Returns or sets the number of columns in the specified slicer. |
| [Parent](parent) { get; } | Returns the Worksheet object that represents the sheet that contains the slicer. Read-only. |
| [Placement](placement) { get; set; } | Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [RowHeight](rowheight) { get; set; } | Returns or sets the height, in points, of each row in the specified slicer. |
| [RowHeightPixel](rowheightpixel) { get; set; } | Returns or sets the height, in pixels, of each row in the specified slicer. |
| [SlicerCache](slicercache) { get; } | Returns the SlicerCache object associated with the slicer. Read-only. |
| [StyleType](styletype) { get; set; } | Specify the type of Built-in slicer style the default type is SlicerStyleLight1 |
| [Title](title) { get; set; } | Specifies the title of the current Slicer object. |
| [TopPixel](toppixel) { get; set; } | Returns or sets the vertical offset of slicer shape from its top row, in pixels. |
| [Width](width) { get; set; } | Returns or sets the width of the specified slicer, in points. |
| [WidthPixel](widthpixel) { get; set; } | Returns or sets the width of the specified slicer, in pixels. |

## Methods

| Name | Description |
| --- | --- |
| [AddPivotConnection](addpivotconnection)(PivotTable) | Adds PivotTable connection. |
| [Refresh](refresh)() | Refreshing the slicer.Meanwhile, Refreshing and Calculating relative PivotTables. |
| [RemovePivotConnection](removepivotconnection)(PivotTable) | Removes PivotTable connection. |

### Examples

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
//do your business
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

### See Also

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
