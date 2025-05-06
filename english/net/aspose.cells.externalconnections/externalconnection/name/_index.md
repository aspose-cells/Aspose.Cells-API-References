---
title: ExternalConnection.Name
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Specifies the name of the connection. Each connection must have a unique name
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/name/
---
## ExternalConnection.Name property

Specifies the name of the connection. Each connection must have a unique name.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;ThisWorkbookDataModel&amp;quot;, connection.Name); //
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET57308.xlsx&quot;);
            var connection = workbook.DataConnections[0];
            Assert.AreEqual(&quot;ModelConnection_ExternalData_1&quot;, connection.Name); // ModelConnection_ExternalData_1, expected: not present
            Console.WriteLine(connection.PowerQueryFormula);

            connection = workbook.DataConnections[1];
            Assert.AreEqual(&quot;Query - aandelenratings&quot;, connection.Name); // Query - aandelenratings
            Assert.AreEqual(&quot;aandelenratings&quot;, connection.PowerQueryFormula.Name); // null, expected: not null

            connection = workbook.DataConnections[2];
            Assert.AreEqual(&quot;ThisWorkbookDataModel&quot;, connection.Name); // 
            Console.WriteLine(connection.PowerQueryFormula);

            var table = workbook.Worksheets[0].QueryTables[0];
            Assert.AreEqual(&quot;Query - aandelenratings&quot;, table.ExternalConnection.Name); // ModelC
            workbook.Save(Constants.destPath + &quot;CELLSNET57308.xlsx&quot;);
        }
```

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


