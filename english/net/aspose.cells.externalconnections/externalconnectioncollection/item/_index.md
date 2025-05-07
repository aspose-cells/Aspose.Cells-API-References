---
title: ExternalConnectionCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnectionCollection property. Gets the ExternalConnection element at the specified index
type: docs
url: /net/aspose.cells.externalconnections/externalconnectioncollection/item/
---
## ExternalConnectionCollection indexer (1 of 2)

Gets the [`ExternalConnection`](../../externalconnection/) element at the specified index.

```csharp
public ExternalConnection this[int index] { get; set; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: connection = workbook.DataConnections[1];
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET57308.xlsx");
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
            workbook.Save(Constants.destPath + "CELLSNET57308.xlsx");
        }
```

### See Also

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ExternalConnectionCollection indexer (2 of 2)

Gets the [`ExternalConnection`](../../externalconnection/) element with the specified name.

```csharp
public ExternalConnection this[string connectionName] { get; }
```

| Parameter | Description |
| --- | --- |
| connectionName | the name of data connection |

### Return Value

The element with the specified name.

### See Also

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


