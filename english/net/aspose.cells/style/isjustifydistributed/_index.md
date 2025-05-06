---
title: Style.IsJustifyDistributed
second_title: Aspose.Cells for .NET API Reference
description: Style property. Indicates if the cells justified or distributed alignment should be used on the last line of text
type: docs
url: /net/aspose.cells/style/isjustifydistributed/
---
## Style.IsJustifyDistributed property

Indicates if the cells justified or distributed alignment should be used on the last line of text.

```csharp
public bool IsJustifyDistributed { get; set; }
```

### Remarks

This is typical for East Asian alignments but not typical in other contexts.

### Examples

```csharp
// Called: Assert.AreEqual(style.IsJustifyDistributed, true);
[Test]
        public void Property_IsJustifyDistributed()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA40732.xlsx&quot;);
            Style style = workbook.Worksheets[0].Cells[&quot;A1&quot;].GetStyle();
            Assert.AreEqual(style.IsJustifyDistributed, true);
            workbook.Save(Constants.destPath + &quot;CELLSJAVA40732.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSJAVA40732.xlsx&quot;);
            style = workbook.Worksheets[0].Cells[&quot;A1&quot;].GetStyle();
            Assert.AreEqual(style.IsJustifyDistributed, true);
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


