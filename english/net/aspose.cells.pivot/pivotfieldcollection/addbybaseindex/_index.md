---
title: PivotFieldCollection.AddByBaseIndex
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldCollection method. Adds a PivotField Object to the specific type PivotFields
type: docs
url: /net/aspose.cells.pivot/pivotfieldcollection/addbybaseindex/
---
## PivotFieldCollection.AddByBaseIndex method

Adds a PivotField Object to the specific type PivotFields.

```csharp
public int AddByBaseIndex(int baseFieldIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | field index in the base PivotFields. |

### Return Value

the index of the PivotField Object in this PivotFields.

### Examples

```csharp
// Called: int newFieldIndex = rowFields.AddByBaseIndex(1); // Adding the &amp;quot;Year&amp;quot; field to the row area
public static void Method_Int32_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[0, 0].Value = &quot;Fruit&quot;;
            worksheet.Cells[1, 0].Value = &quot;Grape&quot;;
            worksheet.Cells[2, 0].Value = &quot;Blueberry&quot;;
            worksheet.Cells[3, 0].Value = &quot;Kiwi&quot;;
            worksheet.Cells[4, 0].Value = &quot;Cherry&quot;;
            worksheet.Cells[5, 0].Value = &quot;Grape&quot;;
            worksheet.Cells[6, 0].Value = &quot;Blueberry&quot;;
            worksheet.Cells[7, 0].Value = &quot;Kiwi&quot;;
            worksheet.Cells[8, 0].Value = &quot;Cherry&quot;;

            worksheet.Cells[0, 1].Value = &quot;Year&quot;;
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[3, 1].Value = 2020;
            worksheet.Cells[4, 1].Value = 2020;
            worksheet.Cells[5, 1].Value = 2021;
            worksheet.Cells[6, 1].Value = 2021;
            worksheet.Cells[7, 1].Value = 2021;
            worksheet.Cells[8, 1].Value = 2021;

            worksheet.Cells[0, 2].Value = &quot;Amount&quot;;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 2].Value = 80;
            worksheet.Cells[5, 2].Value = 90;
            worksheet.Cells[6, 2].Value = 100;
            worksheet.Cells[7, 2].Value = 110;
            worksheet.Cells[8, 2].Value = 120;

            // Add a pivot table to the worksheet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add(&quot;=Sheet1!A1:C9&quot;, &quot;E3&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Fruit&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Column, &quot;Year&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Amount&quot;);

            // Access the RowFields collection
            PivotFieldCollection rowFields = pivotTable.RowFields;

            // Display the count of row fields
            Console.WriteLine(&quot;Row Fields Count: &quot; + rowFields.Count);

            // Access the first row field and display its name
            PivotField firstRowField = rowFields[0];
            Console.WriteLine(&quot;First Row Field Name: &quot; + firstRowField.Name);

            // Add a new field by base index
            int newFieldIndex = rowFields.AddByBaseIndex(1); // Adding the &quot;Year&quot; field to the row area
            Console.WriteLine(&quot;New Field Index: &quot; + newFieldIndex);

            // Clear all fields in the RowFields collection
            rowFields.Clear();
            Console.WriteLine(&quot;Row Fields Count after Clear: &quot; + rowFields.Count);

            // Save the workbook
            workbook.Save(&quot;PivotFieldCollectionExample.xlsx&quot;);
        }
```

### See Also

* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


