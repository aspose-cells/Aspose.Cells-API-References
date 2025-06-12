---
title: LoadFilter.LoadDataFilterOptions
second_title: Aspose.Cells for .NET API Reference
description: LoadFilter property. The filter options to denote what data should be loaded
type: docs
url: /net/aspose.cells/loadfilter/loaddatafilteroptions/
---
## LoadFilter.LoadDataFilterOptions property

The filter options to denote what data should be loaded.

```csharp
public LoadDataFilterOptions LoadDataFilterOptions { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadFilterPropertyLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // Create load options and set filter options
            LoadOptions options = new LoadOptions();
            options.LoadFilter = new LoadFilter(LoadDataFilterOptions.CellData | LoadDataFilterOptions.DefinedNames);

            // Load workbook with the specified options
            Workbook workbook = new Workbook("input.xlsx", options);

            // Save the workbook (demonstrates successful load with specified filters)
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


