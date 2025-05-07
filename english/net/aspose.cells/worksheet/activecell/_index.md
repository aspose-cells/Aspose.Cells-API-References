---
title: Worksheet.ActiveCell
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets or sets the active cell in the worksheet
type: docs
url: /net/aspose.cells/worksheet/activecell/
---
## Worksheet.ActiveCell property

Gets or sets the active cell in the worksheet.

```csharp
public string ActiveCell { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].ActiveCell, "B2");
[Test]
        public void Property_ActiveCell()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].SelectRange(1, 1, 5, 5,true);
            Assert.AreEqual(workbook.Worksheets[0].ActiveCell, "B2");
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


