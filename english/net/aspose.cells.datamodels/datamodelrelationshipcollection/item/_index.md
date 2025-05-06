---
title: DataModelRelationshipCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: DataModelRelationshipCollection property. Gets the relationship
type: docs
url: /net/aspose.cells.datamodels/datamodelrelationshipcollection/item/
---
## DataModelRelationshipCollection indexer

Gets the relationship.

```csharp
public DataModelRelationship this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index. |

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;Employee&amp;quot;, workbook.DataModel.Relationships[0].ForeignKeyTable);
[Test]
        public void Property_Int32_()
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

* class [DataModelRelationship](../../datamodelrelationship/)
* class [DataModelRelationshipCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


