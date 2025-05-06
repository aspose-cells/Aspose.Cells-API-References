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
// Called: LoadDataFilterOptions = LoadDataFilterOptions.Structure;
public override void Property_LoadDataFilterOptions(Worksheet sheet)
            {
                if (sheet.Index == 0)
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.DefinedNames | LoadDataFilterOptions.CellData;
                }
                else
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.Structure;
                }
            }
```

### See Also

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


