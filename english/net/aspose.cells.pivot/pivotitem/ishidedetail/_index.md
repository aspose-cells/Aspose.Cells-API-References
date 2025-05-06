---
title: PivotItem.IsHideDetail
second_title: Aspose.Cells for .NET API Reference
description: PivotItem property. Gets and sets whether the pivot item hides detail
type: docs
url: /net/aspose.cells.pivot/pivotitem/ishidedetail/
---
## PivotItem.IsHideDetail property

Gets and sets whether the pivot item hides detail.

```csharp
[Obsolete("Use PivotItem.IsDetailHidden property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHideDetail { get; set; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use PivotItem.IsDetailHidden property instead. This property will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: pivotItem.IsHideDetail = false;
public static void Property_IsHideDetail()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Category&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;Fruit&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Vegetable&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(&quot;Amount&quot;);
            worksheet.Cells[&quot;B2&quot;].PutValue(50);
            worksheet.Cells[&quot;B3&quot;].PutValue(30);

            // Add a pivot table to the worksheet
            int pivotIndex = worksheet.PivotTables.Add(&quot;=A1:B3&quot;, &quot;E3&quot;, &quot;PivotTable1&quot;);
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Add fields to the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Access the pivot items
            PivotField pivotField = pivotTable.RowFields[0];
            PivotItemCollection pivotItems = pivotField.PivotItems;

            int pivotItemCount = pivotItems.Count;
            Console.WriteLine(&quot;Number of Pivot Items: &quot; + pivotItemCount);
            for(int i = 0; i &lt; pivotItemCount; i++)
            {
                PivotItem pivotItem = pivotItems[i];
                // Print the name of the pivot item
                Console.WriteLine(&quot;Pivot Item Name: &quot; + pivotItem.Name);

                // Set properties
                pivotItem.IsHidden = false;
                pivotItem.Position = 1;
                pivotItem.IsHideDetail = false;

                // Print the value of the pivot item
                Console.WriteLine(&quot;Pivot Item Value: &quot; + pivotItem.Value);

                // Use methods
                string stringValue = pivotItem.GetStringValue();
                double doubleValue = pivotItem.GetDoubleValue();
                DateTime dateTimeValue = pivotItem.GetDateTimeValue();

                Console.WriteLine(&quot;String Value: &quot; + stringValue);
                Console.WriteLine(&quot;Double Value: &quot; + doubleValue);
                Console.WriteLine(&quot;DateTime Value: &quot; + dateTimeValue);
            }

            // Save the workbook
            workbook.Save(&quot;PivotItemExample.xlsx&quot;);
        }
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


