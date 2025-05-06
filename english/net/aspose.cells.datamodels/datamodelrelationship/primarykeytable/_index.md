---
title: DataModelRelationship.PrimaryKeyTable
second_title: Aspose.Cells for .NET API Reference
description: DataModelRelationship property. Gets the name of the primary key table for this relationship
type: docs
url: /net/aspose.cells.datamodels/datamodelrelationship/primarykeytable/
---
## DataModelRelationship.PrimaryKeyTable property

Gets the name of the primary key table for this relationship.

```csharp
public string PrimaryKeyTable { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;Department&amp;quot;, workbook.DataModel.Relationships[0].PrimaryKeyTable);
[Test]
        public void Property_PrimaryKeyTable()
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

* class [DataModelRelationship](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


