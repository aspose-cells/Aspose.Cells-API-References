---
title: "VerticalPageBreakCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "VerticalPageBreakCollection‑egenskap. Hämtar VerticalPageBreak‑elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells/verticalpagebreakcollection/item/
---
## VerticalPageBreakCollection indexer (1 of 2)

Hämtar [`VerticalPageBreak`](../../verticalpagebreak/)‑elementet på det angivna indexet.

```csharp
public VerticalPageBreak this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Det nollbaserade indexet för elementet. |

### Returvärde

Elementet på det angivna indexet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till vertikala sidbrytningar
            worksheet.VerticalPageBreaks.Add(5);
            worksheet.VerticalPageBreaks.Add(10);
            worksheet.VerticalPageBreaks.Add(15);

            // Kom åt och visa sidbrytningar med Item‑egenskapen
            VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;
            Console.WriteLine("Vertical Page Breaks:");
            for (int i = 0; i < vpagebreaks.Count; i++)
            {
                Console.WriteLine($"Break {i + 1}: Column = {vpagebreaks[i].Column}");
            }

            // Ta bort och lägg till igen för att ändra en sidbrytning eftersom Column är skrivskyddad
            int column = vpagebreaks[1].Column;
            vpagebreaks.RemoveAt(1);
            vpagebreaks.Add(12);
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine($"Break 2: Column = {vpagebreaks[1].Column}");
        }
    }
}
```

### Se även

* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## VerticalPageBreakCollection indexer (2 of 2)

Hämtar [`VerticalPageBreak`](../../verticalpagebreak/)‑elementet med det angivna cellnamnet.

```csharp
public VerticalPageBreak this[string cellName] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| cellName | Cellnamn. |

### Returvärde

Elementet med det angivna cellnamnet.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till några vertikala sidbrytningar
            worksheet.VerticalPageBreaks.Add(3);
            worksheet.VerticalPageBreaks.Add(7);

            try
            {
                // Kom åt VerticalPageBreakCollection
                VerticalPageBreakCollection pageBreaks = worksheet.VerticalPageBreaks;

                // Demonstrera åtkomst av objekt med Item‑egenskapen (indexerare)
                Console.WriteLine("Vertical Page Breaks in the worksheet:");
                for (int i = 0; i < pageBreaks.Count; i++)
                {
                    VerticalPageBreak vpb = pageBreaks[i];
                    Console.WriteLine($"Break {i + 1}: Column = {vpb.Column}, StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}");
                }

                // Spara arbetsboken
                workbook.Save("VerticalPageBreakItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [VerticalPageBreak](../../verticalpagebreak/)
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


