---
title: Enum PivotRefreshState
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotRefreshState enum. The state for refreshing pivot tables
type: docs
url: /net/aspose.cells.pivot/pivotrefreshstate/
---
## PivotRefreshState enumeration

The state for refreshing pivot tables.

```csharp
public enum PivotRefreshState
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Success | `0` | Successfully refreshed |
| UnsupportedExternalDataSource | `1` | Refresh failed because the data source is external. |

### Examples

```csharp
// Called: if(workbook.Worksheets[0].PivotTables[0].RefreshData() == PivotRefreshState.UnsupportedExternalDataSource)
public void Type_PivotRefreshState()
        {
            Workbook workbook = new Workbook(Constants.openPivottablePath + &quot;reiswegvergelijking_evolutie_KPI_kopie.xls&quot;);//source sheet
            if(workbook.Worksheets[0].PivotTables[0].RefreshData() == PivotRefreshState.UnsupportedExternalDataSource)
                workbook.Worksheets[0].PivotTables[0].CalculateData();
            workbook.Save(Constants.savePivottablePath + &quot;book_out.xls&quot;);

        }
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


