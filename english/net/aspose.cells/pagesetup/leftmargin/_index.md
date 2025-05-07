---
title: PageSetup.LeftMargin
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the size of the left margin in unit of centimeters
type: docs
url: /net/aspose.cells/pagesetup/leftmargin/
---
## PageSetup.LeftMargin property

Represents the size of the left margin, in unit of centimeters.

```csharp
public double LeftMargin { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(0, workbook.Worksheets[0].PageSetup.LeftMargin);
[Test]
        public void Property_LeftMargin()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet46004.xlsx");
            Assert.AreEqual(0, workbook.Worksheets[0].PageSetup.LeftMargin);
            workbook.Save(Constants.destPath + "CellsNet46004.xlsx");
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


