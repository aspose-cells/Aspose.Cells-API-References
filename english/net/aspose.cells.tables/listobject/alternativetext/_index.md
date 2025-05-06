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
// Called: Assert.AreEqual(&amp;quot;Test&amp;quot;, table.AlternativeText);
[Test]
        public void Property_AlternativeText()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CellsNet46581.xlsx&quot;);
            ListObject table = wb.Worksheets[0].ListObjects[0];
            Assert.AreEqual(&quot;Test&quot;, table.AlternativeText);
            Assert.AreEqual(&quot;aSXADCS&quot;, table.AlternativeDescription);
            wb.Save(Constants.destPath + &quot;CellsNet46581.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CellsNet46581.xlsx&quot;);
            table = wb.Worksheets[0].ListObjects[0];
            Assert.AreEqual(&quot;Test&quot;, table.AlternativeText);
            Assert.AreEqual(&quot;aSXADCS&quot;, table.AlternativeDescription);
            wb.Save(Constants.destPath + &quot;CellsNet46581.xlsb&quot;);
            wb = new Workbook(Constants.destPath + &quot;CellsNet46581.xlsb&quot;);
            table = wb.Worksheets[0].ListObjects[0];
            Assert.AreEqual(&quot;Test&quot;, table.AlternativeText);
            Assert.AreEqual(&quot;aSXADCS&quot;, table.AlternativeDescription);
        }
```

### See Also

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


