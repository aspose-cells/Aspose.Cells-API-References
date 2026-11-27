---
title: "PivotTable.GetHorizontalBreaks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Hämtar listan med radindex för horisontella sidbrytningar i pivottabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/gethorizontalbreaks/
---
## PivotTable.GetHorizontalBreaks method

Hämtar listan med radindex för horisontella sidbrytningar i pivottabellen

```csharp
[Obsolete("Use ivotTable.GetHorizontalPageBreaks() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetHorizontalBreaks()
```

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället PivotTable.GetHorizontalPageBreaks()-metoden. Denna metod kommer att tas bort 12 månader senare från och med december 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Collections;

    public class PivotTableMethodGetHorizontalBreaksDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Beräkna data för att fylla pivottabellen
            pivotTable.CalculateData();

            try
            {
                // Hämta horisontella brytningar (sidbrytningar) för pivottabellen
                ArrayList horizontalBreaks = pivotTable.GetHorizontalBreaks();
                
                Console.WriteLine("Horizontal breaks (row indices):");
                foreach (int rowIndex in horizontalBreaks)
                {
                    Console.WriteLine(rowIndex);
                }

                // Lägg till en sidbrytning på rad 3 för demonstration
                worksheet.HorizontalPageBreaks.Add("A3");
                
                // Hämta uppdaterade horisontella brytningar
                horizontalBreaks = pivotTable.GetHorizontalBreaks();
                Console.WriteLine("\nHorizontal breaks after adding page break:");
                foreach (int rowIndex in horizontalBreaks)
                {
                    Console.WriteLine(rowIndex);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetHorizontalBreaks method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("PivotTableGetHorizontalBreaksDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


