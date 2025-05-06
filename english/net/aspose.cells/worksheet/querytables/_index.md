---
title: Worksheet.QueryTables
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets QueryTableCollection in the worksheet
type: docs
url: /net/aspose.cells/worksheet/querytables/
---
## Worksheet.QueryTables property

Gets [`QueryTableCollection`](../../querytablecollection/) in the worksheet.

```csharp
public QueryTableCollection QueryTables { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(3, workbook.Worksheets[0].QueryTables.Count);
[Test]
        public void Property_QueryTables()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet47154.ods&quot;);
            workbook.Save(Constants.destPath + &quot;CellsNet47154.ods&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet47154.ods&quot;);
            Assert.AreEqual(3, workbook.DataConnections.Count);
            Assert.AreEqual(3, workbook.Worksheets[0].QueryTables.Count);
            Assert.AreEqual(1, workbook.Worksheets[0].ListObjects.Count);
            workbook.Save(Constants.destPath + &quot;CellsNet47154.xlsx&quot;);
        }
```

### See Also

* class [QueryTableCollection](../../querytablecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


