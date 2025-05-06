---
title: AutoFitterOptions.OnlyAuto
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Indicates whether only fit the rows which height are not customed
type: docs
url: /net/aspose.cells/autofitteroptions/onlyauto/
---
## AutoFitterOptions.OnlyAuto property

Indicates whether only fit the rows which height are not customed.

```csharp
public bool OnlyAuto { get; set; }
```

### Examples

```csharp
// Called: OnlyAuto = true
private static void Property_OnlyAuto(Worksheet worksheet)
        {
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                MaxRowHeight = int.MaxValue,
                OnlyAuto = true
            });
        }
```

### See Also

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


