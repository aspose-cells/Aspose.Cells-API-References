---
title: "PivotTable.RefreshData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable metod. Uppdaterar data från dess datakälla till pivotcachen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/refreshdata/
---
## RefreshData() {#refreshdata}

Uppdaterar data från dess datakälla till pivotcachen.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData()
```

### Anmärkningar

Vi kommer att samla data från datakällan till en pivottcache, sedan beräkna datan i cachen till cellerna. Det är bättre att du helt enkelt kan anropa [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) för att uppdatera och beräkna alla pivottabeller i filen, istället för att uppdatera en efter en. OBS: Denna metod är nu föråldrad. Använd istället [`Refresh`](../../pivotcache/refresh/)‑metoden och ta bort den efterföljande [`CalculateData`](../calculatedata/) eftersom denna pivottabell kommer att beräknas när [`PivotCache`](../pivotcache/) uppdateras. Denna metod kommer att tas bort 12 månader senare, från och med juni 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);
            
            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till rad- och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Uppdatera och beräkna pivottabellsdata
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Spara arbetsboken
            workbook.Save("PivotTableRefreshDataDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RefreshData(PivotTableRefreshOption) {#refreshdata_1}

Uppdaterar pivottabellens data och inställningar från dess datakälla med alternativ.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData(PivotTableRefreshOption option)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | PivotTableRefreshOption | The options for refreshing data source of pivot table. |

### Anmärkningar

Vi kommer att samla data från datakällan till en pivottcache, sedan beräkna datan i cachen till cellerna. Det är bättre att du helt enkelt kan anropa [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) för att uppdatera och beräkna alla pivottabeller i filen, istället för att uppdatera en efter en. OBS: Denna metod är nu föråldrad. Använd istället [`Refresh`](../../pivotcache/refresh/)‑metoden och ta bort den efterföljande [`CalculateData`](../calculatedata/) eftersom denna pivottabell kommer att beräknas när [`PivotCache`](../pivotcache/) uppdateras. Denna metod kommer att tas bort 12 månader senare, från och med juni 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Kom åt kalkylbladet som innehåller pivottabellen
            Worksheet worksheet = workbook.Worksheets["PNL_AFS"];
            
            // Hämta den första pivottabellen i kalkylbladet
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Konfigurera uppdateringsalternativ
            PivotTableRefreshOption refreshOptions = new PivotTableRefreshOption();
            refreshOptions.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
            
            // Uppdatera pivottabellens data med angivna alternativ
            pivotTable.RefreshData(refreshOptions);
            pivotTable.CalculateData();
            
            // Spara den modifierade arbetsboken
            workbook.Save("example_modified.xlsx");
        }
    }
}
```

### Se även

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


