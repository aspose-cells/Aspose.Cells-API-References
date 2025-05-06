---
title: Range.CopyValue
second_title: Aspose.Cells for .NET API Reference
description: Range method. Copies cell value from a source range
type: docs
url: /net/aspose.cells/range/copyvalue/
---
## Range.CopyValue method

Copies cell value from a source range.

```csharp
public void CopyValue(Range range)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | Source [`Range`](../) object. |

### Examples

```csharp
// Called: targetRange.CopyValue(sourceRange);
[Test]
        public void Method_Range_()
        {
            Workbook sourceWB = new Workbook(Constants.sourcePath + &quot;CellsCORE149.xlsx&quot;), targetWB = new Workbook();
            Cells sourceCells = sourceWB.Worksheets[0].Cells;
            Cells targetCells = targetWB.Worksheets.Add(sourceWB.Worksheets[0].Name).Cells;
            Aspose.Cells.Range sourceRange = sourceCells.CreateRange(0, 0, sourceCells.MaxRow + 1, sourceCells.MaxColumn + 1);
            Aspose.Cells.Range targetRange = targetCells.CreateRange(0, 0, sourceCells.MaxRow + 1, sourceCells.MaxColumn + 1);
            targetRange.CopyValue(sourceRange);
            targetRange.CopyStyle(sourceRange);
           Assert.AreEqual(sourceCells[&quot;a1&quot;].Value ,  targetCells[&quot;A1&quot;].Value);
            sourceCells = sourceWB.Worksheets[1].Cells;
            targetCells = targetWB.Worksheets.Add(sourceWB.Worksheets[1].Name).Cells;
            sourceRange = sourceCells.CreateRange(0, 0, sourceCells.MaxRow + 1, sourceCells.MaxColumn + 1);
            targetRange = targetCells.CreateRange(0, 0, sourceCells.MaxRow + 1, sourceCells.MaxColumn + 1);
            targetRange.CopyStyle(sourceRange);
            targetRange.CopyValue(sourceRange);
            Assert.AreEqual(sourceCells[&quot;b5&quot;].Value, targetCells[&quot;b5&quot;].Value);
            targetWB.Save(Constants.destPath + &quot;CellsCORE149.xls&quot;);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


