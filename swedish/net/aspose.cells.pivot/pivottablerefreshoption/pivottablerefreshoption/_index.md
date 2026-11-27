---
title: "PivotTableRefreshOption.PivotTableRefreshOption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Konstruktorn för PivotTableRefreshOption. Representerar alternativen för att uppdatera datakällan för pivottabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottablerefreshoption/pivottablerefreshoption/
---
## PivotTableRefreshOption constructor

Representerar alternativen för att uppdatera datakällan för pivottabellen.

```csharp
public PivotTableRefreshOption()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableRefreshOptionMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Apple";
            cells["B2"].Value = "North";            cells["C2"].Value = 1000;
            cells["A3"].Value = "Orange";            cells["B3"].Value = "South";            cells["C3"].Value = 2000;
            cells["A4"].Value = "Banana";            cells["B4"].Value = "East";            cells["C4"].Value = 3000;
            cells["A5"].Value = "Apple";            cells["B5"].Value = "South";            cells["C5"].Value = 4000;
            
            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Skapa och konfigurera uppdateringsalternativ med hjälp av konstruktorn
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption();
            refreshOption.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
            
            // Uppdatera pivottabellen med alternativ
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotTableRefreshDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [PivotTableRefreshOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


