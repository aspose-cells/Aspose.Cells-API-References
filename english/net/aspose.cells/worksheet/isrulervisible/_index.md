---
title: Worksheet.IsRulerVisible
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates whether the ruler is visible. This property is only applied for page break preview
type: docs
url: /net/aspose.cells/worksheet/isrulervisible/
---
## Worksheet.IsRulerVisible property

Indicates whether the ruler is visible. This property is only applied for page break preview.

```csharp
public bool IsRulerVisible { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].IsRulerVisible);
[Test]
        public void Property_IsRulerVisible()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].ViewType = ViewType.PageLayoutView;
            workbook.Worksheets[0].IsRulerVisible = true;
            workbook.Save(Constants.destPath + "CellsCore82_1.xlsb");
            workbook = new Workbook(Constants.destPath + "CellsCore82_1.xlsb");
            Assert.IsTrue(workbook.Worksheets[0].IsRulerVisible);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


