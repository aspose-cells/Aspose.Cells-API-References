---
title: Class Slicer
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Slicers.Slicer class. summary description of Slicer View
type: docs
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
| [AlternativeText](../../aspose.cells.slicers/slicer/alternativetext/) { get; set; } | (**Obsolete.**) Returns or sets the descriptive (alternative) text string of the Slicer object. |
| [Caption](../../aspose.cells.slicers/slicer/caption/) { get; set; } | Returns or sets the caption of the specified slicer. |
| [CaptionVisible](../../aspose.cells.slicers/slicer/captionvisible/) { get; set; } | (**Obsolete.**) Returns or sets whether the header that displays the slicer Caption is visible. The default value is true |
| [ColumnWidth](../../aspose.cells.slicers/slicer/columnwidth/) { get; set; } | Returns or sets the width of each column in the slicer in unit of points. |
| [ColumnWidthPixel](../../aspose.cells.slicers/slicer/columnwidthpixel/) { get; set; } | Gets or sets the width of each column in the slicer, in unit of pixels. |
| [FirstItemIndex](../../aspose.cells.slicers/slicer/firstitemindex/) { get; set; } | Specifies the zero-based index of the first slicer item. |
| [Height](../../aspose.cells.slicers/slicer/height/) { get; set; } | (**Obsolete.**) Returns or sets the height of the specified slicer, in points. |
| [HeightPixel](../../aspose.cells.slicers/slicer/heightpixel/) { get; set; } | (**Obsolete.**) Returns or sets the height of the specified slicer, in pixels. |
| [IsLocked](../../aspose.cells.slicers/slicer/islocked/) { get; set; } | (**Obsolete.**) Indicates whether the slicer shape is locked. |
| [IsPrintable](../../aspose.cells.slicers/slicer/isprintable/) { get; set; } | (**Obsolete.**) Indicates whether the slicer object is printable. |
| [LeftPixel](../../aspose.cells.slicers/slicer/leftpixel/) { get; set; } | (**Obsolete.**) Returns or sets the horizontal offset of slicer shape from its left column, in pixels. |
| [LockedAspectRatio](../../aspose.cells.slicers/slicer/lockedaspectratio/) { get; set; } | (**Obsolete.**) Indicates whether locking aspect ratio. |
| [LockedPosition](../../aspose.cells.slicers/slicer/lockedposition/) { get; set; } | Indicates whether the specified slicer can be moved or resized by using the user interface. |
| [Name](../../aspose.cells.slicers/slicer/name/) { get; set; } | Returns or sets the name of the specified slicer |
| [NumberOfColumns](../../aspose.cells.slicers/slicer/numberofcolumns/) { get; set; } | Returns or sets the number of columns in the specified slicer. The default value is 1. |
| [Parent](../../aspose.cells.slicers/slicer/parent/) { get; } | (**Obsolete.**) Returns the [`Worksheet`](./worksheet/) object which contains this slicer. Read-only. |
| [Placement](../../aspose.cells.slicers/slicer/placement/) { get; set; } | (**Obsolete.**) Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [RowHeight](../../aspose.cells.slicers/slicer/rowheight/) { get; set; } | Returns or sets the height of each row in the specified slicer in unit of points. |
| [RowHeightPixel](../../aspose.cells.slicers/slicer/rowheightpixel/) { get; set; } | Returns or sets the height of each row in the specified slicer, in unit of pixels. |
| [Shape](../../aspose.cells.slicers/slicer/shape/) { get; } | Returns the Shape object associated with the specified slicer. Read-only. |
| [ShowAllItems](../../aspose.cells.slicers/slicer/showallitems/) { get; set; } | Indicates whether to show all items even if there are no data or they are deleted. Default value is true; |
| [ShowCaption](../../aspose.cells.slicers/slicer/showcaption/) { get; set; } | Indicates whether the header of the slicer is visible. The default value is true |
| [ShowMissing](../../aspose.cells.slicers/slicer/showmissing/) { get; set; } | Indicates whether to show items deteleted from the data source. |
| [ShowTypeOfItemsWithNoData](../../aspose.cells.slicers/slicer/showtypeofitemswithnodata/) { get; set; } | Indicates whether to show items deteleted from the data source. |
| [SlicerCache](../../aspose.cells.slicers/slicer/slicercache/) { get; } | Returns the SlicerCache object associated with the slicer. Read-only. |
| [SortOrderType](../../aspose.cells.slicers/slicer/sortordertype/) { get; set; } | Indicates the type of sorting items. |
| [StyleType](../../aspose.cells.slicers/slicer/styletype/) { get; set; } | Specify the type of Built-in slicer style. The default type is SlicerStyleLight1. |
| [Title](../../aspose.cells.slicers/slicer/title/) { get; set; } | (**Obsolete.**) Specifies the title of the current Slicer object. |
| [TopPixel](../../aspose.cells.slicers/slicer/toppixel/) { get; set; } | (**Obsolete.**) Returns or sets the vertical offset of slicer shape from its top row, in pixels. |
| [Width](../../aspose.cells.slicers/slicer/width/) { get; set; } | (**Obsolete.**) Returns or sets the width of the specified slicer, in points. |
| [WidthPixel](../../aspose.cells.slicers/slicer/widthpixel/) { get; set; } | (**Obsolete.**) Returns or sets the width of the specified slicer, in pixels. |
| [Worksheet](../../aspose.cells.slicers/slicer/worksheet/) { get; } | Returns the [`Worksheet`](./worksheet/) object which contains this slicer. Read-only. |

## Methods

| Name | Description |
| --- | --- |
| [AddPivotConnection](../../aspose.cells.slicers/slicer/addpivotconnection/)(PivotTable) | Adds PivotTable connection. |
| [Refresh](../../aspose.cells.slicers/slicer/refresh/)() | Refreshing the slicer. Meanwhile, Refreshing and Calculating PivotTables which this slicer based on. |
| [RemovePivotConnection](../../aspose.cells.slicers/slicer/removepivotconnection/)(PivotTable) | Removes PivotTable connection. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Slicers;
    using Aspose.Cells.Pivot;
    using System;

    public class SlicerDemo
    {
        public static void SlicerExample()
        {
            // Create a new workbook and get the first worksheet
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Populate the worksheet with sample data
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

            // Add a pivot table
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            pivot.RefreshData();
            pivot.CalculateData();

            // Add a slicer
            SlicerCollection slicers = sheet.Slicers;
            int slicerIndex = slicers.Add(pivot, "E12", "fruit");
            Slicer slicer = slicers[slicerIndex];
            slicer.StyleType = SlicerStyleType.SlicerStyleLight2;

            // Set slicer properties
            slicer.Title = "Slicer Title";
            slicer.AlternativeText = "AlternativeText test";
            slicer.IsPrintable = true;
            slicer.IsLocked = false;
            slicer.Placement = Aspose.Cells.Drawing.PlacementType.FreeFloating;
            slicer.LockedAspectRatio = true;
            slicer.LockedPosition = false;
            slicer.Name = "Slicer Name";
            slicer.Caption = "Slicer Caption";
            slicer.CaptionVisible = true;
            slicer.NumberOfColumns = 1;
            slicer.LeftPixel = 2;
            slicer.TopPixel = 6;
            slicer.Width = 100;
            slicer.WidthPixel = 120;
            slicer.Height = 120;
            slicer.HeightPixel = 150;
            slicer.ColumnWidthPixel = 120;
            slicer.ColumnWidth = 80;
            slicer.RowHeightPixel = 30;
            slicer.RowHeight = 20;

            // Refresh the slicer
            slicer.Refresh();

            // Save the workbook
            book.Save("SlicerExample.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


