---
title: "TxtLoadOptions.HeaderColumnsCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtLoadOptions-egenskap. Antalet rubrikkolumner som ska upprepas för utökade blad"
type: docs
url: /sv/net/aspose.cells/txtloadoptions/headercolumnscount/
---
## TxtLoadOptions.HeaderColumnsCount property

Antalet rubrikkolumner som ska upprepas för utökade blad.

```csharp
public int HeaderColumnsCount { get; set; }
```

### Anmärkningar

De rubrikkolumner som anges av den här egenskapen kommer att dupliceras för de utökade bladen. Den här egenskapen gäller endast när [`ExtendToNextSheet`](../extendtonextsheet/) är sann.

### Exempel

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHeaderColumnsCountDemo
    {
        public static void Run()
        {
            // Skapa exempel-CSV-innehåll
            string csvData = "Header1,Header2,Header3,Data1,Data2,Data3\n" +
                            "H1,H2,H3,D1,D2,D3\n" +
                            "A,B,C,D,E,F\n" +
                            "G,H,I,J,K,L";

            // Skapa TxtLoadOptions med HeaderColumnsCount satt till 3
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderColumnsCount = 3, // First 3 columns will be treated as headers
                Encoding = Encoding.UTF8
            };

            // Läs in CSV-data i en arbetsbok
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Demonstrera rubrikkolumner (de första 3 kolumnerna)
                Console.WriteLine("Header Columns:");
                for (int row = 0; row < 2; row++)
                {
                    for (int col = 0; col < options.HeaderColumnsCount; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // Demonstrera datakolumner (återstående kolumner)
                Console.WriteLine("\nData Columns:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = options.HeaderColumnsCount; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }
            }
        }
    }
}
```

### Se även

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


