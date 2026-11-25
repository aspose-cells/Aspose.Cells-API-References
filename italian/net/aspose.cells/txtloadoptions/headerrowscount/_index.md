---
title: "TxtLoadOptions.HeaderRowsCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtLoadOptions. Il conteggio delle righe di intestazione da ripetere per i fogli estesi"
type: docs
url: /it/net/aspose.cells/txtloadoptions/headerrowscount/
---
## TxtLoadOptions.HeaderRowsCount property

Il conteggio delle righe di intestazione da ripetere per i fogli estesi.

```csharp
public int HeaderRowsCount { get; set; }
```

### Osservazioni

Le righe di intestazione specificate da questa proprietà verranno duplicate per quei fogli estesi. Questa proprietà ha effetto solo quando [`ExtendToNextSheet`](../extendtonextsheet/) è true.

### Esempi

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
            // Crea contenuto CSV di esempio
            string csvData = "Header1,Header2,Header3\n" +
                            "Value1,Value2,Value3\n" +
                            "Value4,Value5,Value6\n" +
                            "Value7,Value8,Value9";

            // Crea TxtLoadOptions con HeaderRowsCount impostato a 1
            TxtLoadOptions options = new TxtLoadOptions
            {
                HeaderRowsCount = 1
            };

            // Carica i dati CSV in una cartella di lavoro
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(csvData)))
            {
                Workbook workbook = new Workbook(stream, options);

                // Accedi al primo foglio di lavoro
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Dimostra che la prima riga è trattata come intestazione
                Console.WriteLine("Header Row:");
                for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                {
                    Console.Write(cells[0, col].StringValue + "\t");
                }
                Console.WriteLine("\n");

                // Mostra le righe di dati (saltando l'intestazione)
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

### Vedi anche

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


