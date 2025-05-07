---
title: Picture.Formula
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Gets and sets the data of the formula
type: docs
url: /net/aspose.cells.drawing/picture/formula/
---
## Picture.Formula property

Gets and sets the data of the formula.

```csharp
public string Formula { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("=#REF!$A$2:$F$4", workbook.Worksheets[0].Pictures[0].Formula);
[Test]
        public void Property_Formula()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET45312.xls");
            Assert.AreEqual("=#REF!$A$2:$F$4", workbook.Worksheets[0].Pictures[0].Formula);
            workbook.Worksheets[0].Pictures[0].Formula = workbook.Worksheets[0].Pictures[0].Formula;
            workbook.Save(Constants.destPath + "CELLSNET45312.xls");
            workbook = new Workbook(Constants.destPath + "CELLSNET45312.xls");
            Assert.AreEqual("=#REF!$A$2:$F$4", workbook.Worksheets[0].Pictures[0].Formula);
        }
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


