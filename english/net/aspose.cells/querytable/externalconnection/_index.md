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
// Called: Assert.AreEqual(&amp;quot;Query - aandelenratings&amp;quot;, table.ExternalConnection.Name); // ModelC
[Test]
        public void Property_ExternalConnection()
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

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


