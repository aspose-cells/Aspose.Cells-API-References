---
title: Worksheet.RefreshPivotTables
second_title: Aspose.Cells for .NET API Reference
description: Worksheet method. Refreshes all the PivotTables in this Worksheet
type: docs
url: /net/aspose.cells/worksheet/refreshpivottables/
---
## RefreshPivotTables() {#refreshpivottables_1}

Refreshes all the PivotTables in this Worksheet.

```csharp
public void RefreshPivotTables()
```

### Examples

```csharp
// Called: wb.Worksheets[0].RefreshPivotTables();
[Test]
        public void Method_RefreshPivotTables()
        {
            Workbook wb = new Workbook(Constants.PivotTableSourcePath + &quot;JAVA45913.xlsx&quot;);
            wb.Worksheets[0].RefreshPivotTables();
            Assert.AreEqual(&quot;#N/A&quot;, wb.Worksheets[0].Cells[&quot;H6&quot;].StringValue);
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}

Refreshes all the PivotTables in this Worksheet.

```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The option for refreshing data source of pivot table. |

### See Also

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


