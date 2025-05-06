---
title: Worksheet.IsOutlineShown
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates whether to show outline
type: docs
url: /net/aspose.cells/worksheet/isoutlineshown/
---
## Worksheet.IsOutlineShown property

Indicates whether to show outline.

```csharp
public bool IsOutlineShown { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(v,workbook.Worksheets[0].IsOutlineShown);
private void Property_IsOutlineShown(bool v)
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].IsOutlineShown = v;
            Assert.AreEqual(v,workbook.Worksheets[0].IsOutlineShown);
            workbook.Save(Constants.destPath + &quot;dest.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;dest.xlsx&quot;);
            Assert.AreEqual(v, workbook.Worksheets[0].IsOutlineShown);
            workbook.Save(Constants.destPath + &quot;dest.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;dest.xls&quot;);
            Assert.AreEqual(v, workbook.Worksheets[0].IsOutlineShown);
            workbook.Save(Constants.destPath + &quot;dest.xlsb&quot;);
            workbook = new Workbook(Constants.destPath + &quot;dest.xlsb&quot;);
            Assert.AreEqual(v, workbook.Worksheets[0].IsOutlineShown);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


