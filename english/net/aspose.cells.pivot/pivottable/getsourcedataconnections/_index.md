---
title: PivotTable.GetSourceDataConnections
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Gets the external connection data sources
type: docs
url: /net/aspose.cells.pivot/pivottable/getsourcedataconnections/
---
## PivotTable.GetSourceDataConnections method

Gets the external connection data sources.

```csharp
public ExternalConnection[] GetSourceDataConnections()
```

### Examples

```csharp
// Called: conn = workbook.Worksheets[1].PivotTables[0].GetSourceDataConnections()[0];
public void PivotTable_Method_GetSourceDataConnections()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");

    ExternalConnection conn = workbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
    Assert.AreEqual("WorksheetConnection_Sheet3!$B$2:$C$114", conn.Name);
    Assert.AreEqual(ExternalConnectionClassType.DataModel, conn.ClassType);
   Assert.AreEqual(ConnectionDataSourceType.WorksheetDataModel, conn.SourceType);
   Assert.IsNull(conn.ConnectionFile);
    Assert.IsNull(conn.ConnectionString);

    Assert.AreEqual("Sheet3!$B$2:$C$114", conn.Command);


    conn = workbook.Worksheets[1].PivotTables[0].GetSourceDataConnections()[0];
    Assert.AreEqual("Data3",conn.Command);
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


