---
title: PivotFieldGroupSettings.Type
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldGroupSettings property. Gets the group type of pivot field
type: docs
url: /net/aspose.cells.pivot/pivotfieldgroupsettings/type/
---
## PivotFieldGroupSettings.Type property

Gets the group type of pivot field.

```csharp
public virtual PivotFieldGroupType Type { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Group Type: &amp;quot; + groupSettings.Type);
public static void Property_Type()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[0, 0].Value = &quot;Fruit&quot;;
            worksheet.Cells[1, 0].Value = &quot;Apple&quot;;
            worksheet.Cells[2, 0].Value = &quot;Banana&quot;;
            worksheet.Cells[3, 0].Value = &quot;Cherry&quot;;
            worksheet.Cells[4, 0].Value = &quot;Date&quot;;

            worksheet.Cells[0, 1].Value = &quot;Amount&quot;;
            worksheet.Cells[1, 1].Value = 50;
            worksheet.Cells[2, 1].Value = 60;
            worksheet.Cells[3, 1].Value = 70;
            worksheet.Cells[4, 1].Value = 80;

            // Add a pivot table to the worksheet
            int pivotIndex = worksheet.PivotTables.Add(&quot;=Sheet1!A1:B5&quot;, &quot;E3&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Access the row field
            PivotField rowField = pivotTable.RowFields[0];
            rowField.GroupBy(new CustomPiovtFieldGroupItem[] { new CustomPiovtFieldGroupItem(&quot;TestItemGroup&quot;, new int[] { 0, 1 }) }, true);

            // Access the group settings of the row field
            PivotFieldGroupSettings groupSettings = rowField.GroupSettings;

            // Display the group type of the pivot field
            Console.WriteLine(&quot;Group Type: &quot; + groupSettings.Type);

            // Save the workbook
            workbook.Save(&quot;PivotFieldGroupSettingsExample.xlsx&quot;);
        }
```

### See Also

* enum [PivotFieldGroupType](../../pivotfieldgrouptype/)
* class [PivotFieldGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


