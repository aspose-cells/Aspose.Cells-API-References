---
title: "HyperlinkCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HyperlinkCollection-metod. Ta bort hyperlänken på det angivna indexet i denna samling"
type: docs
url: /sv/net/aspose.cells/hyperlinkcollection/removeat/
---
## HyperlinkCollection.RemoveAt method

Ta bort hyperlänken på det angivna indexet i denna samling.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Det nollbaserade indexet för elementet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till en hyperlänk till cell A1
            sheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Verifiera att hyperlänken finns innan borttagning
            Console.WriteLine("Hyperlinks count before removal: " + sheet.Hyperlinks.Count);
            
            // Ta bort hyperlänken på index 0
            sheet.Hyperlinks.RemoveAt(0);
            
            // Verifiera att hyperlänken har tagits bort
            Console.WriteLine("Hyperlinks count after removal: " + sheet.Hyperlinks.Count);
        }
    }
}
```

### Se även

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


