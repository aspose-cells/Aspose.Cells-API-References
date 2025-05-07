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
// Called: sheet.RefreshPivotTables();
[Test]
        public void Method_RefreshPivotTables()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET45657_";

            Workbook excel = new Workbook(filePath + "test.xlsx");
            Worksheet sheet = excel.Worksheets[0];
            PivotTable pivot = sheet.PivotTables[0];

            pivot.RefreshData();
            //this works 
            pivot.CalculateData();
            //this doesn't work 
            //this also doesn't work 
            sheet.RefreshPivotTables();

            excel = new Workbook(filePath + "test.xltm");
            sheet = excel.Worksheets[0];
            pivot = sheet.PivotTables[0];

            pivot.RefreshData();
            //this works 
            pivot.CalculateData();
            //this doesn't work 
            //this also doesn't work 
            sheet.RefreshPivotTables();
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


