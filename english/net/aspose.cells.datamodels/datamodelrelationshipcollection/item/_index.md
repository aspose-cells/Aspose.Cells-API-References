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
// Called: Assert.AreEqual("Department", workbook.DataModel.Relationships[0].ForeignKeyColumn);
public void DataModelRelationshipCollection_Property_Item()
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

* class [DataModelRelationship](../../datamodelrelationship/)
* class [DataModelRelationshipCollection](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


