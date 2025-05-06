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
// Called: var dataModelSource = pivotTable.GetSourceDataConnections()[0].Command; // expected: Sheet1!$A$1:$B$10, actual: 1
[Test]
        public void Method_GetSourceDataConnections()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET56969.xlsx&quot;);
            var dataModelConnection = workbook.DataConnections.OfType&lt;DataModelConnection&gt;().First();
            var command = dataModelConnection.Command; // expected: Sheet1!$A$1:$B$10, actual: 1
            Assert.AreEqual(&quot;Sheet1!$A$1:$B$10&quot;,command);
            var pivotTable = workbook.Worksheets[0].PivotTables[0];
            var dataSource = pivotTable.DataSource; // null
            var dataModelSource = pivotTable.GetSourceDataConnections()[0].Command; // expected: Sheet1!$A$1:$B$10, actual: 1
            Assert.AreEqual(&quot;Sheet1!$A$1:$B$10&quot;, dataModelSource);
        }
```

### See Also

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


