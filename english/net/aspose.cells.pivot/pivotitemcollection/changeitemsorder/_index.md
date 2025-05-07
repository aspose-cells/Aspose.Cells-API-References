---
title: PivotItemCollection.ChangeitemsOrder
second_title: Aspose.Cells for .NET API Reference
description: PivotItemCollection method. Directly changes the orders of the two items
type: docs
url: /net/aspose.cells.pivot/pivotitemcollection/changeitemsorder/
---
## PivotItemCollection.ChangeitemsOrder method

Directly changes the orders of the two items.

```csharp
[Obsolete("Use PivotItemCollection.SwapItem() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ChangeitemsOrder(int sourceIndex, int destIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | Int32 | The current index |
| destIndex | Int32 | The dest index |

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotItemCollection.SwapItem() method. This method will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: pivotItems.ChangeitemsOrder(0, 2);
public static void Method_Int32_()
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

            worksheet.Cells[0, 1].Value = "Quantity";
            worksheet.Cells[1, 1].Value = 10;
            worksheet.Cells[2, 1].Value = 20;
            worksheet.Cells[3, 1].Value = 30;
            worksheet.Cells[4, 1].Value = 40;

            // Add a pivot table to the worksheet
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity

            // Access the PivotField and its PivotItems
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            // Display the count of pivot items
            Console.WriteLine("Pivot Items Count: " + pivotItems.Count);

            // Iterate through the pivot items and display their names
            foreach (PivotItem item in pivotItems)
            {
                Console.WriteLine("Pivot Item: " + item.Name);
            }

            // Change the order of pivot items
            pivotItems.ChangeitemsOrder(0, 2);

            // Save the workbook
            workbook.Save("PivotItemCollectionExample.xlsx");

            return;
        }
```

### See Also

* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


