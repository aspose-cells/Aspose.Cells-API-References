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
// Called: Assert.AreEqual(&amp;quot;F9&amp;quot;,workbook.Worksheets[1].CellWatches[0].CellName);
[Test]
        public void Property_CellName()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA42625.xlsx&quot;);
            Assert.AreEqual(2, workbook.Worksheets[1].CellWatches.Count);
            Assert.AreEqual(&quot;F9&quot;,workbook.Worksheets[1].CellWatches[0].CellName);
            workbook.Worksheets[1].CellWatches.Add(&quot;A1&quot;);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA42625.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSJAVA42625.xlsx&quot;);
            Assert.AreEqual(3, workbook.Worksheets[1].CellWatches.Count);
        }
```

### See Also

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


