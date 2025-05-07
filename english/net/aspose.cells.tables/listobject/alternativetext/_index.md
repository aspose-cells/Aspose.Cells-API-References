---
title: ListObject.AlternativeText
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets the alternative text
type: docs
url: /net/aspose.cells.tables/listobject/alternativetext/
---
## ListObject.AlternativeText property

Gets and sets the alternative text.

```csharp
public string AlternativeText { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("Test", table.AlternativeText);
[Test]
        public void Property_AlternativeText()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CellsNet46581.xlsx");
            ListObject table = wb.Worksheets[0].ListObjects[0];
            Assert.AreEqual("Test", table.AlternativeText);
            Assert.AreEqual("aSXADCS", table.AlternativeDescription);
            wb.Save(Constants.destPath + "CellsNet46581.xlsx");
            wb = new Workbook(Constants.destPath + "CellsNet46581.xlsx");
            table = wb.Worksheets[0].ListObjects[0];
            Assert.AreEqual("Test", table.AlternativeText);
            Assert.AreEqual("aSXADCS", table.AlternativeDescription);
            wb.Save(Constants.destPath + "CellsNet46581.xlsb");
            wb = new Workbook(Constants.destPath + "CellsNet46581.xlsb");
            table = wb.Worksheets[0].ListObjects[0];
            Assert.AreEqual("Test", table.AlternativeText);
            Assert.AreEqual("aSXADCS", table.AlternativeDescription);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


