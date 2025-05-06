---
title: Worksheet.HasAutofilter
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates whether this worksheet has auto filter
type: docs
url: /net/aspose.cells/worksheet/hasautofilter/
---
## Worksheet.HasAutofilter property

Indicates whether this worksheet has auto filter.

```csharp
public bool HasAutofilter { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].HasAutofilter);
[Test]
        public void Property_HasAutofilter()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-43562.xlsx&quot;);
            workbook.Save(Constants.destPath + &quot;CellsNet43562.ods&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet43562.ods&quot;);
            Assert.IsTrue(workbook.Worksheets[0].HasAutofilter);
            workbook.Save(Constants.destPath + &quot;CellsNet43562.xlsx&quot;);
            
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


