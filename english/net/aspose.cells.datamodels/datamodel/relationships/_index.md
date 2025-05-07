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
// Called: Assert.AreEqual("Department", workbook.DataModel.Relationships[0].ForeignKeyColumn);
[Test]
        public void Property_Relationships()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET56974.xlsx");
            Assert.AreEqual("Employee", workbook.DataModel.Relationships[0].ForeignKeyTable);
            Assert.AreEqual("Department", workbook.DataModel.Relationships[0].ForeignKeyColumn);
            Assert.AreEqual("Department", workbook.DataModel.Relationships[0].PrimaryKeyTable);
            Assert.AreEqual("Department", workbook.DataModel.Relationships[0].PrimaryKeyColumn);
            workbook.Save(Constants.destPath + "CellsNet46694.xlsb");
            workbook = new Workbook(Constants.destPath + "CellsNet46694.xlsb");
            workbook.Save(Constants.destPath + "CellsNet46694.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet46694.xlsx");
            Assert.AreEqual("Employee", workbook.DataModel.Relationships[0].ForeignKeyTable);
            Assert.AreEqual("Department", workbook.DataModel.Relationships[0].ForeignKeyColumn);
            Assert.AreEqual("Department", workbook.DataModel.Relationships[0].PrimaryKeyTable);
            Assert.AreEqual("Department", workbook.DataModel.Relationships[0].PrimaryKeyColumn);
            Assert.AreEqual(2, workbook.DataModel.Tables.Count);
        }
```

### See Also

* class [DataModelRelationshipCollection](../../datamodelrelationshipcollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


