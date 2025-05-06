---
title: ListColumn.Name
second_title: Aspose.Cells for .NET API Reference
description: ListColumn property. Gets and sets the name of the column
type: docs
url: /net/aspose.cells.tables/listcolumn/name/
---
## ListColumn.Name property

Gets and sets the name of the column.

```csharp
public string Name { get; set; }
```

### Remarks

If sets the name of the column, the according cell' value will be changed too.

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;c&amp;quot;, table.ListColumns[0].Name);
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET58080.xls&quot;);
            workbook.Save(Constants.destPath + &quot;CELLSNET58080.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET58080.xls&quot;);
            ListObject table = workbook.Worksheets[0].ListObjects[0];
            Assert.AreEqual(&quot;c&quot;, table.ListColumns[0].Name); 

        }
```

### See Also

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


