---
title: AutoFilter.Range
second_title: Aspose.Cells for .NET API Reference
description: AutoFilter property. Represents the range to which the specified AutoFilter applies
type: docs
url: /net/aspose.cells/autofilter/range/
---
## AutoFilter.Range property

Represents the range to which the specified AutoFilter applies.

```csharp
public string Range { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;A1:B2&amp;quot;,workbook.Worksheets[0].AutoFilter.Range);
[Test]
        public void Property_Range()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSAPP4050.xlsx&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            cells.DeleteColumns(2, 4, true);
            Assert.AreEqual(&quot;A1:B2&quot;,workbook.Worksheets[0].AutoFilter.Range);
            workbook.Save(Constants.destPath + &quot;CELLSAPP4050.xlsx&quot;);
        }
```

### See Also

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


