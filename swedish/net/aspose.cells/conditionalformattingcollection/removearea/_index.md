---
title: "ConditionalFormattingCollection.RemoveArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ConditionalFormattingCollection-metod. Ta bort all villkorsstyrd formatering i området"
type: docs
url: /sv/net/aspose.cells/conditionalformattingcollection/removearea/
---
## ConditionalFormattingCollection.RemoveArea method

Ta bort all villkorlig formatering i intervallet.

```csharp
public void RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRow | Int32 | Startraden i området. |
| startColumn | Int32 | Startkolumnen i området. |
| totalRows | Int32 | Antalet rader i området. |
| totalColumns | Int32 | Antalet kolumner i området. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta den villkorsstyrda formateringssamlingen
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;

            // Lägg till några villkorsstyrda formateringsregler
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddArea(area);

            try
            {
                // Anropa RemoveArea med parametrarna (Int32, Int32, Int32, Int32)
                cfc.RemoveArea(0, 0, 3, 3);

                Console.WriteLine("Conditional formatting removed from area (0,0,3,3)");
                
                // Verifiera effekten genom att kontrollera antalet (detta skulle vara 0 om all formatering togs bort)
                Console.WriteLine($"Remaining conditional formatting areas: {fcc.RangeCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("RemoveAreaWithInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


