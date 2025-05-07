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
// Called: slicer.StyleType = SlicerStyleType.SlicerStyleLight1;
public static void Type_SlicerStyleType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
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

            // Get the slicer collection
            SlicerCollection slicers = sheet.Slicers;

            // Add a slicer to the worksheet
            int slicerIndex = slicers.Add(pivot, "E2", "fruit");

            // Access the slicer
            Slicer slicer = slicers[slicerIndex];

            // Set some properties of the slicer
            slicer.Caption = "Fruit Slicer";
            slicer.StyleType = SlicerStyleType.SlicerStyleLight1;

            // Save the workbook
            workbook.Save("SlicerCollectionExample.xlsx");
        }
```

### See Also

* namespace [Aspose.Cells.Slicers](../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../)


