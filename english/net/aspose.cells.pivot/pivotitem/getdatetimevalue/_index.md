---
title: PivotItem.GetDateTimeValue
second_title: Aspose.Cells for .NET API Reference
description: PivotItem method. Gets the date time value of the pivot item If the value is null it will return DateTime.MinValue
type: docs
url: /net/aspose.cells.pivot/pivotitem/getdatetimevalue/
---
## PivotItem.GetDateTimeValue method

Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue

```csharp
public DateTime GetDateTimeValue()
```

### Examples

```csharp
// Called: DateTime dateTimeValue = pivotItem.GetDateTimeValue();
public static void PivotItem_Method_GetDateTimeValue()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);

            // Add a pivot table to the worksheet
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Access the pivot items
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            int pivotItemCount = pivotItems.Count;
            Console.WriteLine("Number of Pivot Items: " + pivotItemCount);
            for(int i = 0; i < pivotItemCount; i++)
            {
                PivotItem pivotItem = pivotItems[i];
                // Print the name of the pivot item
                Console.WriteLine("Pivot Item Name: " + pivotItem.Name);

                // Set properties
                pivotItem.IsHidden = false;
                pivotItem.Position = 1;
                pivotItem.IsHideDetail = false;

                // Print the value of the pivot item
                Console.WriteLine("Pivot Item Value: " + pivotItem.Value);

                // Use methods
                string stringValue = pivotItem.GetStringValue();
                double doubleValue = pivotItem.GetDoubleValue();
                DateTime dateTimeValue = pivotItem.GetDateTimeValue();

                Console.WriteLine("String Value: " + stringValue);
                Console.WriteLine("Double Value: " + doubleValue);
                Console.WriteLine("DateTime Value: " + dateTimeValue);
            }

            // Save the workbook
            workbook.Save("PivotItemExample.xlsx");
        }
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


