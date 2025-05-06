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
            sheet.Cells[&quot;A1&quot;].PutValue(&quot;Apple&quot;);
            sheet.Cells[&quot;A2&quot;].PutValue(&quot;Banana&quot;);
            sheet.Cells[&quot;A3&quot;].PutValue(&quot;Cherry&quot;);
            sheet.Cells[&quot;A4&quot;].PutValue(&quot;Date&quot;);
            sheet.Cells[&quot;A5&quot;].PutValue(&quot;Elderberry&quot;);

            // Create a CustomFilterCollection
            CustomFilterCollection customFilters = new CustomFilterCollection();

            //// Create a CustomFilter for filtering fruits that start with &apos;A&apos; or &apos;B&apos;
            //CustomFilter filter1 = new CustomFilter()
            //{
            //    FilterOperatorType = FilterOperatorType.Equal,
            //    Criteria = &quot;Apple&quot;
            //};

            //CustomFilter filter2 = new CustomFilter()
            //{
            //    FilterOperatorType = FilterOperatorType.Equal,
            //    Criteria = &quot;Banana&quot;
            //};

            //// Add filters to the collection with &quot;And&quot; relationship
            //customFilters.And = true;

            //// Set criteria for the filters
            //customFilters.Append(filter1);
            //customFilters.Append(filter2);

            // Apply the custom filters to the worksheet
            // Assuming we have a method to apply filters (not defined in the provided code)
            ApplyCustomFilters(sheet, customFilters);

            // Save the workbook
            workbook.Save(&quot;CustomFilterDemo.xlsx&quot;);
            workbook.Save(&quot;CustomFilterDemo.pdf&quot;);
        }
```

### See Also

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


