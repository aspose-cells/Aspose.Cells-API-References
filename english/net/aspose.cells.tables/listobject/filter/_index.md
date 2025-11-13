---
title: ListObject.Filter
second_title: Aspose.Cells for .NET API Reference
description: ListObject method. Filter the table
type: docs
url: /net/aspose.cells.tables/listobject/filter/
---
## ListObject.Filter method

Filter the table.

```csharp
[Obsolete("Use set ListObject.HasAutoFilter property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public AutoFilter Filter()
```

### Remarks

NOTE: This member is now obsolete. Instead,please set ListObject.HasAutoFilter property./// This property will be removed 12 months later since October 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectMethodFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate sample data for list object
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["A3"].PutValue("Smartphone");
            worksheet.Cells["B3"].PutValue(800);
            worksheet.Cells["A4"].PutValue("Monitor");
            worksheet.Cells["B4"].PutValue(250);

            try
            {
                // Create a list object from data range using ListObjects.Add with correct parameters
                int listObjectIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[listObjectIndex];
                
                // Get AutoFilter through Filter method
                AutoFilter autoFilter = listObject.Filter();

                // Apply filter on Price column (index 1) to show items >= 800
                autoFilter.Custom(1, FilterOperatorType.GreaterOrEqual, 800);

                Console.WriteLine("Filter applied successfully. Showing items with Price >= 800.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Filter method: {ex.Message}");
            }

            workbook.Save("ListObjectMethodFilterDemo.xlsx");
        }
    }
}
```

### See Also

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


