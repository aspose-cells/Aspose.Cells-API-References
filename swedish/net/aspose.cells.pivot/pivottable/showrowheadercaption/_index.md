---
title: "PivotTable.ShowRowHeaderCaption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om radhuvudrubriken visas i PivotTable-rapporten. Anger om fältetiketter och filterrullgardiner visas"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showrowheadercaption/
---
## PivotTable.ShowRowHeaderCaption property

Anger om radhuvudrubriken visas i PivotTable-rapporten Anger om fältetiketter och filterrullgardiner visas

```csharp
[Obsolete("Use PivotTable.ShowHeaders property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ShowRowHeaderCaption { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället PivotTable.ShowHeaders-egenskapen. Denna metod kommer att tas bort 12 månader senare från och med april 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowRowHeaderCaptionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och fyll i med exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Lägg till exempeldata för pivottabell
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Demonstrera ShowRowHeaderCaption-egenskapen
            pivotTable.ShowRowHeaderCaption = true;
            Console.WriteLine("Row Header Caption Visible: " + pivotTable.ShowRowHeaderCaption);
            
            // Spara arbetsboken
            workbook.Save("PivotTableShowRowHeaderCaptionDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


