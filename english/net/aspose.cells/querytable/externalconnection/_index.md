---
title: QueryTable.ExternalConnection
second_title: Aspose.Cells for .NET API Reference
description: QueryTable property. Gets the relate external connection
type: docs
url: /net/aspose.cells/querytable/externalconnection/
---
## QueryTable.ExternalConnection property

Gets the relate external connection.

```csharp
public ExternalConnection ExternalConnection { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("Query - aandelenratings", table.ExternalConnection.Name); // ModelC
public void QueryTable_Property_ExternalConnection()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var connection = workbook.DataConnections[0];
    Assert.AreEqual("ModelConnection_ExternalData_1", connection.Name); // ModelConnection_ExternalData_1, expected: not present
    Console.WriteLine(connection.PowerQueryFormula);

    connection = workbook.DataConnections[1];
    Assert.AreEqual("Query - aandelenratings", connection.Name); // Query - aandelenratings
    Assert.AreEqual("aandelenratings", connection.PowerQueryFormula.Name); // null, expected: not null

    connection = workbook.DataConnections[2];
    Assert.AreEqual("ThisWorkbookDataModel", connection.Name); // 
    Console.WriteLine(connection.PowerQueryFormula);

    var table = workbook.Worksheets[0].QueryTables[0];
    Assert.AreEqual("Query - aandelenratings", table.ExternalConnection.Name); // ModelC
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


