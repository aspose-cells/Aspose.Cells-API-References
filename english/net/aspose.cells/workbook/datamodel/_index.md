---
title: Workbook.DataModel
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets data model in the workbook
type: docs
url: /net/aspose.cells/workbook/datamodel/
---
## Workbook.DataModel property

Gets data model in the workbook.

```csharp
public DataModel DataModel { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;Employee&amp;quot;, workbook.DataModel.Relationships[0].ForeignKeyTable);
[Test]
        public void Property_DataModel()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET56974.xlsx&quot;);
            Assert.AreEqual(&quot;Employee&quot;, workbook.DataModel.Relationships[0].ForeignKeyTable);
            Assert.AreEqual(&quot;Department&quot;, workbook.DataModel.Relationships[0].ForeignKeyColumn);
            Assert.AreEqual(&quot;Department&quot;, workbook.DataModel.Relationships[0].PrimaryKeyTable);
            Assert.AreEqual(&quot;Department&quot;, workbook.DataModel.Relationships[0].PrimaryKeyColumn);
            workbook.Save(Constants.destPath + &quot;CellsNet46694.xlsb&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet46694.xlsb&quot;);
            workbook.Save(Constants.destPath + &quot;CellsNet46694.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet46694.xlsx&quot;);
            Assert.AreEqual(&quot;Employee&quot;, workbook.DataModel.Relationships[0].ForeignKeyTable);
            Assert.AreEqual(&quot;Department&quot;, workbook.DataModel.Relationships[0].ForeignKeyColumn);
            Assert.AreEqual(&quot;Department&quot;, workbook.DataModel.Relationships[0].PrimaryKeyTable);
            Assert.AreEqual(&quot;Department&quot;, workbook.DataModel.Relationships[0].PrimaryKeyColumn);
            Assert.AreEqual(2, workbook.DataModel.Tables.Count);
        }
```

### See Also

* class [DataModel](../../../aspose.cells.datamodels/datamodel/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


