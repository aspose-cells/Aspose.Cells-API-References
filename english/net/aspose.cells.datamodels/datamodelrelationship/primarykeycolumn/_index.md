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
public void DataModelRelationship_Property_PrimaryKeyColumn()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual("Employee", workbook.DataModel.Relationships[0].ForeignKeyTable);
    Assert.AreEqual("Department", workbook.DataModel.Relationships[0].ForeignKeyColumn);
    Assert.AreEqual("Department", workbook.DataModel.Relationships[0].PrimaryKeyTable);
    Assert.AreEqual("Department", workbook.DataModel.Relationships[0].PrimaryKeyColumn);
    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
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


