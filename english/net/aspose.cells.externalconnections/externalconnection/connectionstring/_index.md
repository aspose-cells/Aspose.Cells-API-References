---
title: ExternalConnection.ConnectionString
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. The connection information string is used to make contact with an OLE DB or ODBC data source
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/connectionstring/
---
## ExternalConnection.ConnectionString property

The connection information string is used to make contact with an OLE DB or ODBC data source.

```csharp
public virtual string ConnectionString { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(wb.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0].ConnectionString != null);
public void ExternalConnection_Property_ConnectionString()
{
    Workbook wb = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    // wb.Worksheets[0].PivotTables.Clear();
    wb.Save(Constants.PivotTableDestPath + "example.xls");
    wb = new Workbook(Constants.PivotTableDestPath + "example.xls");
    wb.Save(Constants.PivotTableDestPath + "example.xlsx");
    Assert.IsTrue(wb.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0].ConnectionString != null);
    Assert.AreEqual("RegressionTestingForClients TestingTime$",wb.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0].Name);
}
```

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


