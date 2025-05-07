---
title: Cells.MaxDisplayRange
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the max range which includes data merged cells and shapes
type: docs
url: /net/aspose.cells/cells/maxdisplayrange/
---
## Cells.MaxDisplayRange property

Gets the max range which includes data, merged cells and shapes.

```csharp
public Range MaxDisplayRange { get; }
```

### Remarks

Reutrns null if the worksheet is empty since Aspose.Cells 21.5.2.

### Examples

```csharp
// Called: var sourceRange = sourceSheet.Cells.MaxDisplayRange;
private static int Property_MaxDisplayRange(Workbook result, int totalRowCount, Workbook data)
        {
            Worksheet destSheet = result.Worksheets[0];
            foreach (Worksheet sourceSheet in data.Worksheets)
            {

                var sourceRange = sourceSheet.Cells.MaxDisplayRange;

                if (sourceRange == null)
                    continue;
                if (sourceRange.RowCount + totalRowCount > 0x100000)
                {
                    totalRowCount = sourceRange.RowCount + totalRowCount;
                    break;
                }
                var destRange = destSheet.Cells.CreateRange(sourceRange.FirstRow + totalRowCount, sourceRange.FirstColumn,
                                    sourceRange.RowCount, sourceRange.ColumnCount);
                destRange.Copy(sourceRange);
                destRange.CopyStyle(sourceRange);
                destSheet.ConditionalFormattings.Copy(sourceSheet.ConditionalFormattings);
                totalRowCount += sourceRange.RowCount;
                // removeSheetNameLs.Add(sourceSheet.Name);
            }
            return totalRowCount;
        }
```

### See Also

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


