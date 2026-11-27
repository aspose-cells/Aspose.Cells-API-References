---
title: "Hyperlink.Area"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Hyperlink‑egenskap. Hämtar området för hyperlänken"
type: docs
url: /sv/net/aspose.cells/hyperlink/area/
---
## Hyperlink.Area property

Hämtar intervallet för hyperlänken.

```csharp
public CellArea Area { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Main Menu");
            worksheet.Cells["A3"].PutValue("Chapter 1");
            worksheet.Cells["A4"].PutValue("Chapter 2");
            
            // Lägg till hyperlänkar
            int hyperlinkIndex1 = worksheet.Hyperlinks.Add("A3", 1, 1, "Sheet2!A1");
            int hyperlinkIndex2 = worksheet.Hyperlinks.Add("A4", 1, 1, "Sheet3!A1");

            // Åtkomst till hyperlänkar och demonstrera användning av Area‑egenskapen
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
            
            string chapter2Address = "";
            foreach (Hyperlink link in hyperlinks)
            {
                // Kontrollera om hyperlänken finns i cell A4 med hjälp av Area‑egenskapen
                if (link.Area.StartRow == 3 && link.Area.StartColumn == 0)
                {
                    chapter2Address = link.Address;
                    break;
                }
            }

            Console.WriteLine("Chapter 2 hyperlink address: " + chapter2Address);
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


