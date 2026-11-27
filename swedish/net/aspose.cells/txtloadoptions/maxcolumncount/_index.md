---
title: "TxtLoadOptions.MaxColumnCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtLoadOptions‑egenskap. Det maximala antalet kolumner som ska importeras för ett blad"
type: docs
url: /sv/net/aspose.cells/txtloadoptions/maxcolumncount/
---
## TxtLoadOptions.MaxColumnCount property

Det maximala antalet kolumner som ska importeras för ett blad.

```csharp
public int MaxColumnCount { get; set; }
```

### Anmärkningar

De kolumner som överskrider denna gräns kommer att ignoreras eller utökas till nästa blad enligt [`ExtendToNextSheet`](../extendtonextsheet/). Detta antal inkluderar rubrikkolumnerna ([`HeaderColumnsCount`](../headercolumnscount/)). Det maximala värdet är kolumngränsen för motsvarande filformat, till exempel för xlsx‑fil är det 16384. Om denna egenskap inte har angetts eller det angivna värdet inte är positivt, används också den maximala gränsen.

### Exempel

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxColumnCountDemo
    {
        public static void Run()
        {
            // Skapa exempel-CSV-innehåll
            string content = "A,B,C,D,E,F,G,H,I,J,K\n" +
                            "1,2,3,4,5,6,7,8,9,10,11\n" +
                            "a,b,c,d,e,f,g,h,i,j,k";

            // Skapa TxtLoadOptions med MaxColumnCount satt till 5
            TxtLoadOptions options = new TxtLoadOptions
            {
                MaxColumnCount = 5  // Only load first 5 columns
            };

            // Läs in CSV‑filen med begränsade kolumner
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Skriv ut den inlästa datan (endast de första 5 kolumnerna ska vara närvarande)
                Console.WriteLine("Data loaded with MaxColumnCount = 5:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // Verifiera att endast 5 kolumner har lästs in
                Console.WriteLine($"\nMax loaded columns: {cells.MaxDataColumn + 1}");
            }
        }
    }
}
```

### Se även

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


