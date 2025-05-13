---
title: ExternalConnection.PowerQueryFormula
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Gets the definition of power query formula
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/powerqueryformula/
---
## ExternalConnection.PowerQueryFormula property

Gets the definition of power query formula.

```csharp
public virtual PowerQueryFormula PowerQueryFormula { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("aandelenratings", connection.PowerQueryFormula.Name); // null, expected: not null
public void ExternalConnection_Property_PowerQueryFormula()
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

* class [PowerQueryFormula](../../../aspose.cells.querytables/powerqueryformula/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


