---
title: DataModel.Relationships
second_title: Aspose.Cells for .NET API Reference
description: DataModel property. Gets all relationships of the tables in the data model
type: docs
url: /net/aspose.cells.datamodels/datamodel/relationships/
---
## DataModel.Relationships property

Gets all relationships of the tables in the data model.

```csharp
public DataModelRelationshipCollection Relationships { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;Department&amp;quot;, workbook.DataModel.Relationships[0].PrimaryKeyColumn);
[Test]
        public void Property_Relationships()
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

* class [DataModelRelationshipCollection](../../datamodelrelationshipcollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


