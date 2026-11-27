---
title: "PivotTable.SelectArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Välj ett område i pivottabellvyn"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/selectarea/
---
## PivotTable.SelectArea method

Välj ett område i pivottabellvyn.

```csharp
public PivotAreaCollection SelectArea(CellArea ca)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | CellArea | Cellområdet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableMethodSelectAreaWithCellAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Beräkna data
            pivotTable.CalculateData();

            // Definiera cellområdet som ska väljas
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.StartColumn = 4;
            area.EndRow = 5;
            area.EndColumn = 6;

            try
            {
                // Anropa metoden SelectArea med parametern CellArea
                PivotAreaCollection selectedAreas = pivotTable.SelectArea(area);
                
                Console.WriteLine("SelectArea method executed successfully. Selected areas count: " + selectedAreas.Count);
                
                // Spara arbetsboken för att visa effekten
                workbook.Save("PivotTableSelectAreaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SelectArea method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PivotAreaCollection](../../pivotareacollection/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


