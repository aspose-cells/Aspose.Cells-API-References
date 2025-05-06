---
title: Worksheet.VisibilityType
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates the visible state for this sheet
type: docs
url: /net/aspose.cells/worksheet/visibilitytype/
---
## Worksheet.VisibilityType property

Indicates the visible state for this sheet.

```csharp
public VisibilityType VisibilityType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[2].VisibilityType, VisibilityType.Visible);
[Test]
        public void Property_VisibilityType()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();
            workbook.Worksheets[0].VisibilityType = VisibilityType.Hidden;
            workbook.Worksheets[1].VisibilityType = VisibilityType.VeryHidden;
            workbook.Worksheets[2].VisibilityType = VisibilityType.Visible;
            workbook.Save(Constants.destPath + &quot;CELLSNET15431.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET15431.xls&quot;);
            Assert.AreEqual(workbook.Worksheets[0].VisibilityType, VisibilityType.Hidden);
            Assert.AreEqual(workbook.Worksheets[1].VisibilityType, VisibilityType.VeryHidden);
            Assert.AreEqual(workbook.Worksheets[2].VisibilityType, VisibilityType.Visible);
        }
```

### See Also

* enum [VisibilityType](../../visibilitytype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


