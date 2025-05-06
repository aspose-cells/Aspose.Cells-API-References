---
title: Enum SlicerStyleType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Slicers.SlicerStyleType enum. Specify the style of slicer view
type: docs
url: /net/aspose.cells.slicers/slicerstyletype/
---
## SlicerStyleType enumeration

Specify the style of slicer view

```csharp
public enum SlicerStyleType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| SlicerStyleLight1 | `0` | built-in light style one |
| SlicerStyleLight2 | `1` | built-in light style two |
| SlicerStyleLight3 | `2` | built-in light style three |
| SlicerStyleLight4 | `3` | built-in light style four |
| SlicerStyleLight5 | `4` | built-in light style five |
| SlicerStyleLight6 | `5` | built-in light style six |
| SlicerStyleOther1 | `6` | built-in style other one |
| SlicerStyleOther2 | `7` | built-in style other two |
| SlicerStyleDark1 | `8` | built-in dark style one |
| SlicerStyleDark2 | `9` | built-in dark style tow |
| SlicerStyleDark3 | `10` | built-in dark style three |
| SlicerStyleDark4 | `11` | built-in dark style four |
| SlicerStyleDark5 | `12` | built-in dark style five |
| SlicerStyleDark6 | `13` | built-in dark style six |
| Custom | `14` | user-defined style, unsupported for now |

### Examples

```csharp
// Called: slicer.StyleType = SlicerStyleType.SlicerStyleLight2;
public static void Type_SlicerStyleType()
        {
            // Create a new workbook and get the first worksheet
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Populate the worksheet with sample data
            cells[0, 0].Value = &quot;fruit&quot;;
            cells[1, 0].Value = &quot;grape&quot;;
            cells[2, 0].Value = &quot;blueberry&quot;;
            cells[3, 0].Value = &quot;kiwi&quot;;
            cells[4, 0].Value = &quot;cherry&quot;;
            cells[5, 0].Value = &quot;grape&quot;;
            cells[6, 0].Value = &quot;blueberry&quot;;
            cells[7, 0].Value = &quot;kiwi&quot;;
            cells[8, 0].Value = &quot;cherry&quot;;

            cells[0, 1].Value = &quot;year&quot;;
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = &quot;amount&quot;;
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
            int pivotIndex = pivots.Add(&quot;=Sheet1!A1:C9&quot;, &quot;A12&quot;, &quot;TestPivotTable&quot;);
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, &quot;fruit&quot;);
            pivot.AddFieldToArea(PivotFieldType.Column, &quot;year&quot;);
            pivot.AddFieldToArea(PivotFieldType.Data, &quot;amount&quot;);
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            pivot.RefreshData();
            pivot.CalculateData();

            // Add a slicer
            SlicerCollection slicers = sheet.Slicers;
            int slicerIndex = slicers.Add(pivot, &quot;E12&quot;, &quot;fruit&quot;);
            Slicer slicer = slicers[slicerIndex];
            slicer.StyleType = SlicerStyleType.SlicerStyleLight2;

            // Set slicer properties
            slicer.Title = &quot;Slicer Title&quot;;
            slicer.AlternativeText = &quot;AlternativeText test&quot;;
            slicer.IsPrintable = true;
            slicer.IsLocked = false;
            slicer.Placement = Aspose.Cells.Drawing.PlacementType.FreeFloating;
            slicer.LockedAspectRatio = true;
            slicer.LockedPosition = false;
            slicer.Name = &quot;Slicer Name&quot;;
            slicer.Caption = &quot;Slicer Caption&quot;;
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
            book.Save(&quot;SlicerExample.xlsx&quot;);
        }
```

### See Also

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


