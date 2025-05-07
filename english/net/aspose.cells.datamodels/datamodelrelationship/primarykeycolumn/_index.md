---
title: DataModelRelationship.PrimaryKeyColumn
second_title: Aspose.Cells for .NET API Reference
description: DataModelRelationship property. Gets the name of the primary key table column for this relationship
type: docs
url: /net/aspose.cells.datamodels/datamodelrelationship/primarykeycolumn/
---
## DataModelRelationship.PrimaryKeyColumn property

Gets the name of the primary key table column for this relationship.

```csharp
public string PrimaryKeyColumn { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("Department", workbook.DataModel.Relationships[0].PrimaryKeyColumn);
[Test]
        public void Property_PrimaryKeyColumn()
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

* class [DataModelRelationship](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


