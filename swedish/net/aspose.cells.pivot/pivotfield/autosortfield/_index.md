---
title: "PivotField.AutoSortField"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField egenskap. Representerar indexet för fältet som sorteras automatiskt. 1 betyder PivotField själv, andra betyder positionen för datafälten."
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/autosortfield/
---
## PivotField.AutoSortField property

Representerar indexet för fältet som sorteras automatiskt. -1 betyder PivotField själv, andra betyder positionen för datafälten.

```csharp
[Obsolete("Use PivotField.SortSetting.SortBy property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoSortField { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället PivotField.SortSetting.SortBy-egenskapen eller PivotField.SortBy()-metoden. Denna metod kommer att tas bort 12 månader senare, från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoSortFieldDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Branch";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "North";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "South";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "East";
            cells["B4"].Value = 800;
            cells["A5"].Value = "West";
            cells["B5"].Value = 1200;

            // Lägg till pivottabell
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Branch");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Hämta pivotfältet
            PivotField pivotField = pivotTable.RowFields["Branch"];

            // Konfigurera automatisk sortering
            pivotField.IsAutoSort = true;
            pivotField.IsAscendSort = true;
            pivotField.AutoSortField = 0; // Sort by first data field (Sales)

            // Beräkna data och uppdatera
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotFieldAutoSortDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


