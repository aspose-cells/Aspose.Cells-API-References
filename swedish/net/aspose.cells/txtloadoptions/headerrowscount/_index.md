---
title: "TxtLoadOptions.HeaderRowsCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TxtLoadOptions egenskap. Antalet rubrikrader som ska upprepas för utökade blad"
type: docs
url: /sv/net/aspose.cells/txtloadoptions/headerrowscount/
---
## TxtLoadOptions.HeaderRowsCount property

Antalet rubrikrader som ska upprepas för utökade blad.

```csharp
public int HeaderRowsCount { get; set; }
```

### Anmärkningar

Rubrikraderna som anges av denna egenskap kommer att dupliceras för de utökade bladen. Denna egenskap träder endast i kraft när [`ExtendToNextSheet`](../extendtonextsheet/) är true.

### Exempel

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyHeaderRowsCountDemo
    {
        public static void Run()
        {
            // Skapa exempel-CSV-innehåll
            string csvData = "Header1,Header2,Header3\n" +
                            "Value1,Value2,Value3\n" +
                            "Value4,Value5,Value6\n" +
                            "Value7,Value8,Value9";

            // Skapa TxtLoadOptions med HeaderRowsCount satt till 1
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderRowsCount = 1
            };

            // Läs in CSV-data i en arbetsbok
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);

                // Åtkomst till det första kalkylbladet
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Visa att den första raden behandlas som rubrik
                Console.WriteLine("Header Row:");
                for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                {
                    Console.Write(cells[0, col].StringValue + "\t");
                }
                Console.WriteLine("\n");

                // Visa datarader (hoppar över rubriken)
                Console.WriteLine("Data Rows:");
                for (int row = 1; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
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


