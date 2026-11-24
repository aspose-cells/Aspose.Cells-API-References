---
title: "TxtLoadOptions.HeaderColumnsCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtLoadOptions‑Eigenschaft. Die Anzahl der Kopfspalten, die für erweiterte Blätter wiederholt werden"
type: docs
url: /de/net/aspose.cells/txtloadoptions/headercolumnscount/
---
## TxtLoadOptions.HeaderColumnsCount property

Die Anzahl der Kopfzeilen-Spalten, die für erweiterte Blätter wiederholt werden.

```csharp
public int HeaderColumnsCount { get; set; }
```

### Hinweise

Die durch diese Eigenschaft angegebenen Kopfspalten werden für die erweiterten Blätter dupliziert. Diese Eigenschaft wirkt nur, wenn [`ExtendToNextSheet`](../extendtonextsheet/) true ist.

### Beispiele

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
            // Erstelle Beispiel‑CSV‑Inhalt
            string csvData = "Header1,Header2,Header3,Data1,Data2,Data3\n" +
                            "H1,H2,H3,D1,D2,D3\n" +
                            "A,B,C,D,E,F\n" +
                            "G,H,I,J,K,L";

            // Erstelle TxtLoadOptions mit HeaderColumnsCount auf 3 gesetzt
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderColumnsCount = 3, // First 3 columns will be treated as headers
                Encoding = Encoding.UTF8
            };

            // Lade die CSV-Daten in eine Arbeitsmappe
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Demonstriere Kopfspalten (erste 3 Spalten)
                Console.WriteLine("Header Columns:");
                for (int row = 0; row < 2; row++)
                {
                    for (int col = 0; col < options.HeaderColumnsCount; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // Demonstriere Daten­spalten (verbleibende Spalten)
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

### Siehe auch

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


