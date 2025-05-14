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
// Called: ExternalConnection connection = pivot.ExternalConnectionDataSource;
public void PivotTable_Property_ExternalConnectionDataSource()
{
    string filePath = Constants.PivotTableSourcePath + @"NET47141_";

    Workbook wb = new Workbook(filePath + "Sample Pivot Table.xlsx");
    PivotTable pivot = wb.Worksheets["SQL Pivot Table"].PivotTables[0];
    ExternalConnection connection = pivot.ExternalConnectionDataSource;
    Assert.AreEqual(connection.Name, "HARSH StudentDB StudentReg");

}
```

### See Also

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


