---
title: "Worksheet.Hyperlinks"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar HyperlinkCollection‑samlingen"
type: docs
url: /sv/net/aspose.cells/worksheet/hyperlinks/
---
## Worksheet.Hyperlinks property

Hämtar [`HyperlinkCollection`](../../hyperlinkcollection/) samlingen.

```csharp
public HyperlinkCollection Hyperlinks { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHyperlinksDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en hyperlänk i kalkylbladet
            worksheet.Hyperlinks.Add(0, 0, 1, 1, @"https://www.aspose.com");
            
            // Spara arbetsboken
            workbook.Save("HyperlinksDemo.xlsx");
            
            // Läs in den sparade arbetsboken för att verifiera hyperlänken
            Workbook loadedWorkbook = new Workbook("HyperlinksDemo.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            // Visa hyperlänkens adress
            Console.WriteLine("Hyperlink Address: " + loadedWorksheet.Hyperlinks[0].Address);
        }
    }
}
```

### Se även

* class [HyperlinkCollection](../../hyperlinkcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


