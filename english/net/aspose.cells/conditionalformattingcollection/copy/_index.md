---
title: ConditionalFormattingCollection.Copy
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingCollection method. Copies conditional formatting
type: docs
url: /net/aspose.cells/conditionalformattingcollection/copy/
---
## ConditionalFormattingCollection.Copy method

Copies conditional formatting.

```csharp
public void Copy(ConditionalFormattingCollection cfs)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cfs | ConditionalFormattingCollection | The conditional formatting |

### Examples

```csharp
// Called: destSheet.ConditionalFormattings.Copy(sourceSheet.ConditionalFormattings);
private static int Method_ConditionalFormattingCollection_(Workbook result, int totalRowCount, Workbook data)
        {
            Worksheet destSheet = result.Worksheets[0];
            foreach (Worksheet sourceSheet in data.Worksheets)
            {

                var sourceRange = sourceSheet.Cells.MaxDisplayRange;

                if (sourceRange == null)
                    continue;
                if (sourceRange.RowCount + totalRowCount &gt; 0x100000)
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

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


