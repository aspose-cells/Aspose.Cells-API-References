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

            Workbook wb = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET47911.xlsb&quot;);
            wb.Save(Constants.PivotTableDestPath + &quot;CELLSNET47911.xlsx&quot;);
            wb = new Workbook(Constants.PivotTableDestPath + &quot;CELLSNET47911.xlsx&quot;);
            Assert.AreEqual(1,wb.DataModel.Tables.Count);
            wb.Save(Constants.PivotTableDestPath + &quot;CELLSNET47911.xlsb&quot;);
        }
```

### See Also

* class [DataModelTableCollection](../../datamodeltablecollection/)
* class [DataModel](../)
* namespace [Aspose.Cells.DataModels](../../../aspose.cells.datamodels/)
* assembly [Aspose.Cells](../../../)


