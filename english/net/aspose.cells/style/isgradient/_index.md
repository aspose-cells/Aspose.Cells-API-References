---
title: Style.IsGradient
second_title: Aspose.Cells for .NET API Reference
description: Style property. Indicates whether the cell shading is a gradient pattern
type: docs
url: /net/aspose.cells/style/isgradient/
---
## Style.IsGradient property

Indicates whether the cell shading is a gradient pattern.

```csharp
public bool IsGradient { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].Cells[&amp;quot;A5&amp;quot;].GetStyle().IsGradient, &amp;quot;A5.Style should be Gradient&amp;quot;);
[Test]
        public void Property_IsGradient()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;ConditionalFormattings\\CellsNet42271.xlsb&quot;);
            Assert.AreEqual(3, workbook.Worksheets[0].ConditionalFormattings.Count, &quot;CFS.Count&quot;);
            Assert.IsTrue(workbook.Worksheets[0].Cells[&quot;A5&quot;].GetStyle().IsGradient, &quot;A5.Style should be Gradient&quot;);

        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


