---
title: LoadOptions.LoadFilter
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions property. The filter to denote how to load data
type: docs
url: /net/aspose.cells/loadoptions/loadfilter/
---
## LoadOptions.LoadFilter property

The filter to denote how to load data.

```csharp
public LoadFilter LoadFilter { get; set; }
```

### Examples

```csharp
// Called: loadOptions.LoadFilter = new CustomLoadFilter();
public static void Property_LoadFilter()
        {
            // Create a new LoadOptions instance
            LoadOptions loadOptions = new LoadOptions();

            // Create a custom LoadFilter implementation
            loadOptions.LoadFilter = new CustomLoadFilter();

            // Load the workbook with the specified load options
            Workbook workbook = new Workbook("LoadDataFilterOptionsExample_original.xlsx", loadOptions);

            // Save the workbook to verify the loaded data
            workbook.Save("LoadDataFilterOptionsExample.xlsx");
        }
```

### See Also

* class [LoadFilter](../../loadfilter/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


