---
title: "PivotField.HideDetail"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Anger om detaljerna för alla PivotItems i ett pivottabellfält ska döljas. Det vill säga kollapsa/expandera detta fält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/hidedetail/
---
## PivotField.HideDetail method

Anger om detaljerna för alla PivotItems i ett pivottabellfält ska döljas. Det vill säga kollapsa/expandera detta fält.

```csharp
[Obsolete("Use PivotItemsCollection.HideAllDetails() and UnhideAllDetails() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void HideDetail(bool isHiddenDetail)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| isHiddenDetail | Boolean | Om detaljen för pivottfältet ska döljas. |

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotItemsCollection.HideAllDetails() och UnhideAllDetails()-metoden. Denna metod kommer att tas bort 12 månader senare från och med november 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodHideDetailWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Country");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Japan");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("USA");
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["A4"].PutValue("UK");
            sheet.Cells["B4"].PutValue(3000);

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Dölj detaljer för det första radfältet
            PivotField rowField = pivotTable.RowFields[0];
            rowField.HideDetail(true);
            
            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("HideDetailDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


