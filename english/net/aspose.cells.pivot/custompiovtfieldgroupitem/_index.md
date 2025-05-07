---
title: Class CustomPiovtFieldGroupItem
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.CustomPiovtFieldGroupItem class. Represents an item of custom grouped field
type: docs
url: /net/aspose.cells.pivot/custompiovtfieldgroupitem/
---
## CustomPiovtFieldGroupItem class

Represents an item of custom grouped field.

```csharp
public class CustomPiovtFieldGroupItem
```

## Constructors

| Name | Description |
| --- | --- |
| [CustomPiovtFieldGroupItem](custompiovtfieldgroupitem/)(string, int[]) | The constructor of custom group item of pivot field. |

### Examples

```csharp
// Called: rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1 }) }, true);
public static void Type_CustomPiovtFieldGroupItem()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[3, 0].Value = "Cherry";
            worksheet.Cells[4, 0].Value = "Date";

            worksheet.Cells[0, 1].Value = "Amount";
            worksheet.Cells[1, 1].Value = 50;
            worksheet.Cells[2, 1].Value = 60;
            worksheet.Cells[3, 1].Value = 70;
            worksheet.Cells[4, 1].Value = 80;

            // Add a pivot table to the worksheet
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Access the row field
            PivotField rowField = pivotTable.RowFields[0];
            rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem("TestItemGroup", new int[] { 0, 1 }) }, true);

            // Access the group settings of the row field
            PivotFieldGroupSettings groupSettings = rowField.GroupSettings;

            // Display the group type of the pivot field
            Console.WriteLine("Group Type: " + groupSettings.Type);

            // Save the workbook
            workbook.Save("PivotFieldGroupSettingsExample.xlsx");
        }
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


