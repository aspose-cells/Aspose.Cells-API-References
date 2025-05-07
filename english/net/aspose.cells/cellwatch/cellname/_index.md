---
title: CellWatch.CellName
second_title: Aspose.Cells for .NET API Reference
description: CellWatch property. Gets and sets the name of the cell
type: docs
url: /net/aspose.cells/cellwatch/cellname/
---
## CellWatch.CellName property

Gets and sets the name of the cell.

```csharp
public string CellName { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("F9",workbook.Worksheets[1].CellWatches[0].CellName);
[Test]
        public void Property_CellName()
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

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


