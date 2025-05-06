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
// Called: pivotField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem(&amp;quot;TestItemGroup&amp;quot;, new int[] { 0, 1}) }, true);
public static void Type_CustomPiovtFieldGroupItem()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Adding some sample data
            worksheet.Cells[0, 0].PutValue(&quot;Item&quot;);
            worksheet.Cells[0, 1].PutValue(&quot;Quantity&quot;);
            worksheet.Cells[1, 0].PutValue(&quot;A&quot;);
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue(&quot;B&quot;);
            worksheet.Cells[2, 1].PutValue(15);
            worksheet.Cells[3, 0].PutValue(&quot;A&quot;);
            worksheet.Cells[3, 1].PutValue(10);
            worksheet.Cells[4, 0].PutValue(&quot;B&quot;);
            worksheet.Cells[4, 1].PutValue(15);

            // Add a pivot table to the worksheet
            int pivotIndex = worksheet.PivotTables.Add(&quot;=A1:B5&quot;, &quot;D1&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Set row and data fields
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Accessing the row field
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem(&quot;TestItemGroup&quot;, new int[] { 0, 1}) }, true);

            // Create an instance of PivotDiscreteGroupSettings
            PivotDiscreteGroupSettings groupSettings = pivotField.GroupSettings as PivotDiscreteGroupSettings;

            // Set the group type to Discrete (This property is read-only)
            // Display the current group type
            Console.WriteLine(&quot;Group Type: &quot; + groupSettings.Type);

            // Save the workbook
            workbook.Save(&quot;PivotDiscreteGroupSettingsExample.xlsx&quot;);

            return;
        }
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


