---
title: DataModel.Tables
second_title: Aspose.Cells for .NET API Reference
description: DataModel property. Gets all tables in the data model
type: docs
url: /net/aspose.cells.datamodels/datamodel/tables/
---
## DataModel.Tables property

Gets all tables in the data model.

```csharp
public DataModelTableCollection Tables { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1,wb.DataModel.Tables.Count);
[Test]
        public void Property_Tables()
        {

            Workbook wb = new Workbook(Constants.PivotTableSourcePath + "CELLSNET47911.xlsb");
            wb.Save(Constants.PivotTableDestPath + "CELLSNET47911.xlsx");
            wb = new Workbook(Constants.PivotTableDestPath + "CELLSNET47911.xlsx");
            Assert.AreEqual(1,wb.DataModel.Tables.Count);
            wb.Save(Constants.PivotTableDestPath + "CELLSNET47911.xlsb");
        }
```

### See Also

* class [DataModelTableCollection](../../datamodeltablecollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


