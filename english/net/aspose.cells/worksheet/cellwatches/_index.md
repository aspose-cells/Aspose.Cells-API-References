---
title: Worksheet.CellWatches
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets collection of cells on this worksheet being watched in the watch window
type: docs
url: /net/aspose.cells/worksheet/cellwatches/
---
## Worksheet.CellWatches property

Gets collection of cells on this worksheet being watched in the 'watch window'.

```csharp
public CellWatchCollection CellWatches { get; }
```

### Examples

```csharp
// Called: workbook.Worksheets[1].CellWatches.Add("A1");
[Test]
        public void Property_CellWatches()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA42625.xlsx");
            Assert.AreEqual(2, workbook.Worksheets[1].CellWatches.Count);
            Assert.AreEqual("F9",workbook.Worksheets[1].CellWatches[0].CellName);
            workbook.Worksheets[1].CellWatches.Add("A1");
            workbook.Save(Constants.destPath + "CELLSJAVA42625.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSJAVA42625.xlsx");
            Assert.AreEqual(3, workbook.Worksheets[1].CellWatches.Count);
        }
```

### See Also

* class [CellWatchCollection](../../cellwatchcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


