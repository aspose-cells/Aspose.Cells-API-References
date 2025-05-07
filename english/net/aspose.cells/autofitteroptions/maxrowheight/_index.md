---
title: AutoFitterOptions.MaxRowHeight
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Gets and sets the max row heightin unit of Point when autofitting rows
type: docs
url: /net/aspose.cells/autofitteroptions/maxrowheight/
---
## AutoFitterOptions.MaxRowHeight property

Gets and sets the max row height(in unit of Point) when autofitting rows.

```csharp
public double MaxRowHeight { get; set; }
```

### Examples

```csharp
// Called: MaxRowHeight = int.MaxValue,
private static void Property_MaxRowHeight(Worksheet worksheet)
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


