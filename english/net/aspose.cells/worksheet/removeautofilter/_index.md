---
title: Worksheet.RemoveAutoFilter
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Removes the auto filter of the worksheet
type: docs
url: /net/aspose.cells/worksheet/removeautofilter/
---
## Worksheet.RemoveAutoFilter method

Removes the auto filter of the worksheet.

```csharp
public void RemoveAutoFilter()
```

### Examples

```csharp
// Called: d.Worksheets[0].RemoveAutoFilter();
[Test]
        public void Method_RemoveAutoFilter()
        {
            Workbook d = new Workbook(Constants.sourcePath + &quot;CellsNet57060.xlsx&quot;);
           Assert.IsTrue(d.Worksheets[0].Cells.Rows[6].IsHidden);
            Assert.IsTrue(d.Worksheets[0].Cells.Rows[19].IsHidden);
            d.Worksheets[0].RemoveAutoFilter();
            Assert.IsFalse(d.Worksheets[0].Cells.Rows[6].IsHidden);
            Assert.IsTrue(d.Worksheets[0].Cells.Rows[19].IsHidden);
            d.Save(Constants.destPath + &quot;CellsNet57060.xlsx&quot;);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


