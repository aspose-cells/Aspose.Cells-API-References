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
// Called: Assert.IsTrue(workbook.Worksheets[0].Cells["A5"].GetStyle().IsGradient, "A5.Style should be Gradient");
[Test]
        public void Property_IsGradient()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "ConditionalFormattings\\CellsNet42271.xlsb");
            Assert.AreEqual(3, workbook.Worksheets[0].ConditionalFormattings.Count, "CFS.Count");
            Assert.IsTrue(workbook.Worksheets[0].Cells["A5"].GetStyle().IsGradient, "A5.Style should be Gradient");

        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


