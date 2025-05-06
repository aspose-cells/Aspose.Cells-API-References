---
title: AutoFitterOptions.AutoFitMergedCellsType
second_title: Aspose.Cells for .NET API Reference
description: AutoFitterOptions property. Gets and set the type of auto fitting row height of merged cells
type: docs
url: /net/aspose.cells/autofitteroptions/autofitmergedcellstype/
---
## AutoFitterOptions.AutoFitMergedCellsType property

Gets and set the type of auto fitting row height of merged cells.

```csharp
public AutoFitMergedCellsType AutoFitMergedCellsType { get; set; }
```

### Remarks

Excel defaults to ignore merged cells when fitting the row height, so Aspose.Cells works as MS Excel default. Please set this type to change the way of auto fitting row height of merged cells.

### Examples

```csharp
// Called: AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
private static void Property_AutoFitMergedCellsType(Worksheet worksheet)
        {
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                MaxRowHeight = int.MaxValue,
                OnlyAuto = true
            });

            worksheet.AutoFitColumns(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                MaxRowHeight = int.MaxValue,
                OnlyAuto = true
            });
        }
```

### See Also

* enum [AutoFitMergedCellsType](../../autofitmergedcellstype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


