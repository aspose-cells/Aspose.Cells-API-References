---
title: "TxtLoadOptions.HeaderRowsCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtLoadOptions-Eigenschaft. Die Anzahl der Kopfzeilen, die für erweiterte Blätter wiederholt werden sollen"
type: docs
url: /de/net/aspose.cells/txtloadoptions/headerrowscount/
---
## TxtLoadOptions.HeaderRowsCount property

Die Anzahl der Kopfzeilen-Zeilen, die für erweiterte Blätter wiederholt werden.

```csharp
public int HeaderRowsCount { get; set; }
```

### Hinweise

Die durch diese Eigenschaft angegebenen Kopfzeilen werden für diese erweiterten Blätter dupliziert. Diese Eigenschaft wirkt nur, wenn [`ExtendToNextSheet`](../extendtonextsheet/) true ist.

### Beispiele

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
            // Erstelle Beispiel‑CSV‑Inhalt
            string csvData = "Header1,Header2,Header3\n" +
                            "Value1,Value2,Value3\n" +
                            "Value4,Value5,Value6\n" +
                            "Value7,Value8,Value9";

            // Erstelle TxtLoadOptions mit HeaderRowsCount auf 1 gesetzt
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderRowsCount = 1
            };

            // Lade die CSV-Daten in eine Arbeitsmappe
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);

                // Greife auf das erste Arbeitsblatt zu
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Zeige, dass die erste Zeile als Kopfzeile behandelt wird
                Console.WriteLine("Header Row:");
                for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                {
                    Console.Write(cells[0, col].StringValue + "\t");
                }
                Console.WriteLine("\n");

                // Zeige Datenzeilen (Kopfzeile überspringend)
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

### Siehe auch

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


