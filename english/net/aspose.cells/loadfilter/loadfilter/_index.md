---
title: LoadFilter.LoadFilter
second_title: Aspose.Cells for .NET API Reference
description: LoadFilter constructor. Constructs one LoadFilter with default filter options LoadDataFilterOptions.All
type: docs
url: /net/aspose.cells/loadfilter/loadfilter/
---
## LoadFilter() {#constructor}

Constructs one LoadFilter with default filter options LoadDataFilterOptions.All.

```csharp
public LoadFilter()
```

### Examples

```csharp
// Called: LoadFilter filter = new LoadFilter();
private void LoadFilter_Constructor(string path, int limit)
        {
            LoadFilter filter = new LoadFilter();
            InterrupHandler handler = new InterrupHandler(limit, filter);
            Workbook wb = new Workbook(path,
                new LoadOptions() { LoadFilter = filter, LightCellsDataHandler = handler });
            Assert.IsTrue(handler.Exceeded, "Dataset's size should exceed the limit");
            int count = 0;
            foreach (Worksheet sheet in wb.Worksheets)
            {
                count += sheet.Cells.Count;
            }
            Assert.AreEqual(count, limit, path + ": the cell count");
        }
```

### See Also

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadFilter(LoadDataFilterOptions) {#constructor_1}

Constructs one LoadFilter with given filter options.

```csharp
public LoadFilter(LoadDataFilterOptions opts)
```

| Parameter | Type | Description |
| --- | --- | --- |
| opts | LoadDataFilterOptions | the default filter options |

### Examples

```csharp
namespace AsposeCellsExamples.LoadFilterMethodCtorWithLoadDataFilterOptionsDemo
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodCtorWithLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Prepare data for the method parameters (LoadDataFilterOptions)
            LoadDataFilterOptions filterOptions = LoadDataFilterOptions.CellData | LoadDataFilterOptions.Chart;

            try
            {
                // Call the #ctor method with the specific parameter types
                LoadFilter loadFilter = new LoadFilter(filterOptions);

                // Process or display the result
                Console.WriteLine("LoadFilter created successfully with LoadDataFilterOptions: " + filterOptions);

                // Show the effect of the method call
                Console.WriteLine("LoadDataFilterOptions set to: " + loadFilter.LoadDataFilterOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LoadFilter: {ex.Message}");
            }

            // Save the result
            workbook.Save("LoadFilterCtorWithLoadDataFilterOptionsDemo.xlsx");
        }
    }
}
```

### See Also

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


