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
// Called: Assert.AreEqual(workBook.Worksheets[1].CodeName,&amp;quot;FakeCodeName&amp;quot;);
[Test]
        public void Property_CodeName()
        {

            Workbook workBook = new Aspose.Cells.Workbook(Constants.sourcePath + &quot;CellsNet5179.xlsx&quot;);
             Assert.AreEqual(workBook.Worksheets[0].CodeName,&quot;Feuil1&quot;);
             Assert.AreEqual(workBook.Worksheets[1].CodeName,&quot;FakeCodeName&quot;);


            workBook.Worksheets.Add(&quot;NewWorkSheetAspose&quot;);
             Assert.AreEqual(workBook.Worksheets[2].CodeName,&quot;Sheet1&quot;);


            VbaProject f = workBook.VbaProject;
            Assert.AreEqual(workBook.Worksheets[0].CodeName, &quot;Feuil1&quot;);
            Assert.AreEqual(workBook.Worksheets[1].CodeName, &quot;FakeCodeName&quot;);
            Assert.AreEqual(workBook.Worksheets[2].CodeName, &quot;Sheet1&quot;);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


