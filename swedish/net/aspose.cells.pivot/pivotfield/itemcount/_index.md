---
title: "PivotField.ItemCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField egenskap. Hämtar antalet basobjekt i detta pivotfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/itemcount/
---
## PivotField.ItemCount property

Hämtar antalet basobjekt i detta pivotfält.

```csharp
[Obsolete("Use PivotField.PivotItems.Count instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ItemCount { get; }
```

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotField.PivotItems.Count‑egenskap. Denna metod kommer att tas bort 12 månader senare sedan augusti 20268. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyItemCountDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["A5"].PutValue("Vegetable");
            worksheet.Cells["A6"].PutValue("Fruit");
            worksheet.Cells["A7"].PutValue("Vegetable");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["B5"].PutValue(120);
            worksheet.Cells["B6"].PutValue(180);
            worksheet.Cells["B7"].PutValue(90);

            // Lägg till pivottabell
            int index = worksheet.PivotTables.Add("A1:B7", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Hämta pivotfältet och visa dess objektantal
            PivotField pivotField = pivotTable.RowFields[0];
            Console.WriteLine("Item count in pivot field: " + pivotField.ItemCount);
            
            // Spara arbetsboken
            workbook.Save("PivotFieldItemCountDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


