---
title: "HorizontalPageBreakCollection.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HorizontalPageBreakCollection-egenskap. Hämtar HorizontalPageBreak-elementet på det angivna indexet"
type: docs
url: /sv/net/aspose.cells/horizontalpagebreakcollection/item/
---
## HorizontalPageBreakCollection indexer (1 of 2)

Hämtar [`HorizontalPageBreak`](../../horizontalpagebreak/) elementet på det angivna indexet.

```csharp
public HorizontalPageBreak this[int index] { get; }
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
    public class HorizontalPageBreakCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till horisontella sidbrytningar
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            // Åtkomst till sidbrytningar med Item-egenskapen
            HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
            Console.WriteLine("First page break row: " + firstBreak.Row);
            
            // Modifiera celler som påverkar sidbrytningar
            worksheet.Cells.DeleteRows(0, 2);
            
            // Verifiera att sidbrytningen justerades
            Console.WriteLine("First page break after row deletion: " + worksheet.HorizontalPageBreaks[0].Row);
        }
    }
}
```

### Se även

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HorizontalPageBreakCollection indexer (2 of 2)

Hämtar [`HorizontalPageBreak`](../../horizontalpagebreak/) elementet med det angivna cellnamnet.

```csharp
public HorizontalPageBreak this[string cellName] { get; }
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
    using System;
    using Aspose.Cells;

    public class HorizontalPageBreakCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till ett par horisontella sidbrytningar med olika överlagringar
                worksheet.HorizontalPageBreaks.Add(5);          // break after row index 5
                worksheet.HorizontalPageBreaks.Add("D5");      // break at cell D5 (row index 4)

                // ----- Åtkomst via heltalsindex (Item[int]) -----
                // Item-egenskapen är indexeraren, så vi använder []-syntaxen
                HorizontalPageBreak firstBreak = worksheet.HorizontalPageBreaks[0];
                Console.WriteLine("First break row (int index): " + firstBreak.Row);

                // ----- Åtkomst via strängnyckel (Item[string]) -----
                // Hämta sidbrytningen som lades till med cellnamnet "D5"
                HorizontalPageBreak breakByCell = worksheet.HorizontalPageBreaks["D5"];
                Console.WriteLine("Break added with \"D5\" is at row: " + breakByCell.Row);

                // Spara arbetsboken för att verifiera att sidbrytningarna har sparats
                workbook.Save("HorizontalPageBreaks_ItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Se även

* class [HorizontalPageBreak](../../horizontalpagebreak/)
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


