---
title: "PivotField.FilterByValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField metod. Filtrerar efter värden i datapivotfältet"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/filterbyvalue/
---
## PivotField.FilterByValue method

Filtrerar efter värden för data-pivotfält.

```csharp
public PivotFilter FilterByValue(int valueFieldIndex, PivotFilterType type, double value1, 
    double value2)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| valueFieldIndex | Int32 | Index för värdefältet i värdeområdet. |
| typ | PivotFilterType | Typen av filtreringsdata. |
| value1 | Double | Värdet för filtervillkoret |
| value2 | Double | Det övre gränsvärdet för mellanfiltervillkoret |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodFilterByValueWithInt32PivotFilterTypeDoubleDoubDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["B2"].Value = 2.5;
            worksheet.Cells["B3"].Value = 1.8;
            worksheet.Cells["B4"].Value = 3.2;
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["C2"].Value = 100;
            worksheet.Cells["C3"].Value = 150;
            worksheet.Cells["C4"].Value = 80;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Hämta pivotfältet
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Anropa FilterByValue‑metoden med parametrarna (Int32, PivotFilterType, Double, Double)
                // Filtrera produkter där Kvantitet (fältindex 1) är mellan 90 och 160
                PivotFilter filter = pivotField.FilterByValue(1, PivotFilterType.ValueBetween, 90.0, 160.0);

                Console.WriteLine("FilterByValue method executed successfully");
                Console.WriteLine($"Filter type: {filter.FilterType}");
                Console.WriteLine($"Value field index: {filter.ValueFieldIndex}");

                // Uppdatera pivottabellen för att visa ändringarna
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FilterByValue method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("PivotFieldMethodFilterByValueDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


