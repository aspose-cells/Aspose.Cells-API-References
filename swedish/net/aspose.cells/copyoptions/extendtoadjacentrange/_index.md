---
title: "CopyOptions.ExtendToAdjacentRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CopyOptions property. Anger om intervall ska utökas när intervallet kopieras till ett intilliggande intervall"
type: docs
url: /sv/net/aspose.cells/copyoptions/extendtoadjacentrange/
---
## CopyOptions.ExtendToAdjacentRange property

Anger om områden ska utökas när området kopieras till ett intilliggande område.

```csharp
public bool ExtendToAdjacentRange { get; set; }
```

### Anmärkningar

Om det är sant, utökas endast hyperlänkens intervall, utan att lägga till en ny hyperlänk när hyperlänkar kopieras till intilliggande rader.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyExtendToAdjacentRangeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Lägg till en hyperlänk till cell A1
            ws.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Skapa kopieringsalternativ och sätt ExtendToAdjacentRange till true
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ExtendToAdjacentRange = true;

            // Kopiera rad 0 till rad 1 med kopieringsalternativen
            ws.Cells.CopyRows(ws.Cells, 0, 1, 1, copyOptions);

            // Verifiera att hyperlänken utökades till det intilliggande intervallet
            Console.WriteLine("Hyperlink count after copy: " + ws.Hyperlinks.Count);
        }
    }
}
```

### Se även

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


