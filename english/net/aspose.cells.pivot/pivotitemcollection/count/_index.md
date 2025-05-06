---
title: PivotItemCollection.Count
second_title: Aspose.Cells for .NET API Reference
description: PivotItemCollection property. Gets the count of the pivot items
type: docs
url: /net/aspose.cells.pivot/pivotitemcollection/count/
---
## PivotItemCollection.Count property

Gets the count of the pivot items.

```csharp
public int Count { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Pivot Items Count: &amp;quot; + pivotItems.Count);
public static void Property_Count()
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

            worksheet.Cells[0, 1].Value = &quot;Quantity&quot;;
            worksheet.Cells[1, 1].Value = 10;
            worksheet.Cells[2, 1].Value = 20;
            worksheet.Cells[3, 1].Value = 30;
            worksheet.Cells[4, 1].Value = 40;

            // Add a pivot table to the worksheet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add(&quot;=Sheet1!A1:B5&quot;, &quot;E3&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity

            // Access the PivotField and its PivotItems
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            // Display the count of pivot items
            Console.WriteLine(&quot;Pivot Items Count: &quot; + pivotItems.Count);

            // Iterate through the pivot items and display their names
            foreach (PivotItem item in pivotItems)
            {
                Console.WriteLine(&quot;Pivot Item: &quot; + item.Name);
            }

            // Change the order of pivot items
            pivotItems.ChangeitemsOrder(0, 2);

            // Save the workbook
            workbook.Save(&quot;PivotItemCollectionExample.xlsx&quot;);

            return;
        }
```

### See Also

* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


