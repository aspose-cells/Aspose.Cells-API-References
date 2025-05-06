---
title: Cells.StandardHeightInch
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets or sets the default row height in this worksheet in unit of inches
type: docs
url: /net/aspose.cells/cells/standardheightinch/
---
## Cells.StandardHeightInch property

Gets or sets the default row height in this worksheet, in unit of inches.

```csharp
public double StandardHeightInch { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(12.75 / 72, workbook.Worksheets[0].Cells.StandardHeightInch);
[Test]
        public void Property_StandardHeightInch()
        {
            Workbook workbook = new Workbook();
            Assert.AreEqual(12.75 / 72, workbook.Worksheets[0].Cells.StandardHeightInch);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


