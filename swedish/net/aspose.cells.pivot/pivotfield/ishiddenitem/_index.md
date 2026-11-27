---
title: "PivotField.IsHiddenItem"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-metod. Anger om den specifika PivotItem är dold"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/ishiddenitem/
---
## PivotField.IsHiddenItem method

Anger om den specifika PivotItem är dold.

```csharp
[Obsolete("Use PivotField.PivotItems[int].IsHidden instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsHiddenItem(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Indexet för pivotItem i pivotField. |

### Returvärde

om det specifika PivotItem är dolt

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället egenskapen PivotField.PivotItems[int].IsHidden. Denna metod kommer att tas bort 12 månader senare från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodIsHiddenItemWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok och lägg till exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Country";
            worksheet.Cells["A2"].Value = "USA";
            worksheet.Cells["A3"].Value = "Canada";
            worksheet.Cells["A4"].Value = "UK";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Skapa pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            PivotField rowField = pivotTable.RowFields[0];
            
            // Dölj objektet på index 1 (Canada)
            rowField.HideItem(1, true);
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Kontrollera om objektet på index 1 är dolt
            bool isHidden = rowField.IsHiddenItem(1);
            Console.WriteLine("Is item at index 1 hidden? " + isHidden);
            
            // Spara arbetsboken
            workbook.Save("PivotFieldIsHiddenItemDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


