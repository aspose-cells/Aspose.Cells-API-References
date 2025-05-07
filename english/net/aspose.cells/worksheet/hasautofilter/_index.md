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
            Workbook workbook = new Workbook(Constants.HtmlSourcePath + "CELLSJAVA45034.htm");
            Assert.IsTrue(workbook.Worksheets[0].HasAutofilter);
            workbook.Save(Constants.HtmlDestPath + "CELLSJAVA45034.html");
            workbook = new Workbook(Constants.HtmlDestPath + "CELLSJAVA45034.html");
            Assert.IsTrue(workbook.Worksheets[0].HasAutofilter);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


