---
title: "PivotField.ShowCompact"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField‑egenskap. Anger om etiketter för nästa fält ska visas i samma kolumn i pivottabellvyn. Endast för radfält."
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/showcompact/
---
## PivotField.ShowCompact property

Anger om etiketter för nästa fält ska visas i samma kolumn i pivottabellvyn. Endast för radfält.

```csharp
[Obsolete("Use PivotField.ShowInCompactForm instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ShowCompact { get; set; }
```

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotField.ShowInCompactForm‑egenskapen. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowCompactDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Apple");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Orange");
            worksheet.Cells["A6"].PutValue("Grape");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["B5"].PutValue(250);
            worksheet.Cells["B6"].PutValue(300);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A7", "A1:B6", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält och konfigurera ShowCompact
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[fieldIndex];
            rowField.ShowInOutlineForm = true;
            rowField.ShowCompact = true;
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Beräkna och uppdatera pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotFieldShowCompactDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


