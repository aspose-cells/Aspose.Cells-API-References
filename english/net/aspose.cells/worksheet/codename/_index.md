---
title: Worksheet.CodeName
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets worksheet code name
type: docs
url: /net/aspose.cells/worksheet/codename/
---
## Worksheet.CodeName property

Gets worksheet code name.

```csharp
public string CodeName { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workBook.Worksheets[2].CodeName,"Sheet1");
[Test]
        public void Property_CodeName()
        {

            Workbook workBook = new Aspose.Cells.Workbook(Constants.sourcePath + "CellsNet5179.xlsx");
             Assert.AreEqual(workBook.Worksheets[0].CodeName,"Feuil1");
             Assert.AreEqual(workBook.Worksheets[1].CodeName,"FakeCodeName");


            workBook.Worksheets.Add("NewWorkSheetAspose");
             Assert.AreEqual(workBook.Worksheets[2].CodeName,"Sheet1");


            VbaProject f = workBook.VbaProject;
            Assert.AreEqual(workBook.Worksheets[0].CodeName, "Feuil1");
            Assert.AreEqual(workBook.Worksheets[1].CodeName, "FakeCodeName");
            Assert.AreEqual(workBook.Worksheets[2].CodeName, "Sheet1");
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


