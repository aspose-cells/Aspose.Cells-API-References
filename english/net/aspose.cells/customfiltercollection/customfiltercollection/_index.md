---
title: CustomFilterCollection.CustomFilterCollection
second_title: Aspose.Cells for .NET API Reference
description: CustomFilterCollection constructor. Constructs new instance
type: docs
url: /net/aspose.cells/customfiltercollection/customfiltercollection/
---
## CustomFilterCollection constructor

Constructs new instance.

```csharp
public CustomFilterCollection()
```

### Examples

```csharp
// Called: CustomFilterCollection customFilters = new CustomFilterCollection();
public static void CustomFilterCollection_Constructor()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells["A1"].PutValue("Apple");
            sheet.Cells["A2"].PutValue("Banana");
            sheet.Cells["A3"].PutValue("Cherry");
            sheet.Cells["A4"].PutValue("Date");
            sheet.Cells["A5"].PutValue("Elderberry");

            // Create a CustomFilterCollection
            CustomFilterCollection customFilters = new CustomFilterCollection();

            //// Create a CustomFilter for filtering fruits that start with 'A' or 'B'
            //CustomFilter filter1 = new CustomFilter()
            //{
            //    FilterOperatorType = FilterOperatorType.Equal,
            //    Criteria = "Apple"
            //};

            //CustomFilter filter2 = new CustomFilter()
            //{
            //    FilterOperatorType = FilterOperatorType.Equal,
            //    Criteria = "Banana"
            //};

            //// Add filters to the collection with "And" relationship
            //customFilters.And = true;

            //// Set criteria for the filters
            //customFilters.Append(filter1);
            //customFilters.Append(filter2);

            // Apply the custom filters to the worksheet
            // Assuming we have a method to apply filters (not defined in the provided code)
            ApplyCustomFilters(sheet, customFilters);

            // Save the workbook
            workbook.Save("CustomFilterDemo.xlsx");
            workbook.Save("CustomFilterDemo.pdf");
        }
```

### See Also

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


