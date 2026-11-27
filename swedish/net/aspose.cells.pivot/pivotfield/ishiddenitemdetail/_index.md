---
title: "PivotField.IsHiddenItemDetail"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Anger om detaljerna för den specifika PivotItem ska döljas"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/ishiddenitemdetail/
---
## PivotField.IsHiddenItemDetail method

Anger om detaljerna för den specifika PivotItem ska döljas..

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsDetailHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHiddenItemDetail(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Indexet för pivotItem i pivotField. |

### Returvärde

om den specifika PivotItem har dolda detaljer

### Anmärkningar

OBS: Den här metoden är nu föråldrad. Använd istället PivotField.PivotItems[int].IsDetailHidden-egenskapen. Denna metod kommer att tas bort 12 månader senare, från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodIsHiddenItemDetailWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Country";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Japan";
            cells["A3"].Value = "Japan";
            cells["A4"].Value = "USA";
            cells["A5"].Value = "USA";
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;
            cells["B5"].Value = 4000;

            // Lägg till pivottabell
            int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Hämta pivottfältet
            PivotField pivotField = pivotTable.RowFields[0];
            
            // Dölj objektets detaljer för index 1 (USA)
            pivotField.HideItemDetail(1, true);
            
            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Kontrollera om objektets detaljer är dolda
            Console.WriteLine("Is item at index 1 hidden? " + pivotField.IsHiddenItemDetail(1));
            
            // Spara arbetsbok
            workbook.Save("PivotFieldIsHiddenItemDetailDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


