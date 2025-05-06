---
title: ListObject.AlternativeDescription
second_title: Aspose.Cells for .NET API Reference
description: ListObject property. Gets and sets the alternative description
type: docs
url: /net/aspose.cells.tables/listobject/alternativedescription/
---
## ListObject.AlternativeDescription property

Gets and sets the alternative description.

```csharp
public string AlternativeDescription { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;aSXADCS&amp;quot;, table.AlternativeDescription);
[Test]
        public void Property_AlternativeDescription()
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


