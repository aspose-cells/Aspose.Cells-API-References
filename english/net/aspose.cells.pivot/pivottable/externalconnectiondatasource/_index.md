---
title: PivotTable.ExternalConnectionDataSource
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets the external connection data source
type: docs
url: /net/aspose.cells.pivot/pivottable/externalconnectiondatasource/
---
## PivotTable.ExternalConnectionDataSource property

Gets the external connection data source.

```csharp
[Obsolete("Use PivotTable.GetSourceDataConnections() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ExternalConnection ExternalConnectionDataSource { get; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use PivotTable.GetSourceDataConnections() method. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: DBConnection exConn = workbook.Worksheets[2].PivotTables[0].ExternalConnectionDataSource as DBConnection;
[Test]
        public void Property_ExternalConnectionDataSource()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET-47141.xlsx&quot;);
            DBConnection exConn = workbook.Worksheets[2].PivotTables[0].ExternalConnectionDataSource as DBConnection;
           Assert.IsTrue(!string.IsNullOrEmpty(exConn.ConnectionInfo));
            workbook.Save(Constants.PivotTableDestPath + &quot;CellsNet47141.xlsx&quot;);
        }
```

### See Also

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


