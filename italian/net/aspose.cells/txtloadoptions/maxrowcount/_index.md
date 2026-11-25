---
title: "TxtLoadOptions.MaxRowCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtLoadOptions. Il numero massimo di righe da importare per un foglio"
type: docs
url: /it/net/aspose.cells/txtloadoptions/maxrowcount/
---
## TxtLoadOptions.MaxRowCount property

Il conteggio massimo di righe da importare per un foglio.

```csharp
public int MaxRowCount { get; set; }
```

### Osservazioni

Le righe che superano questo limite verranno ignorate o estese al foglio successivo secondo [`ExtendToNextSheet`](../extendtonextsheet/). Questo conteggio include le righe di intestazione ([`HeaderRowsCount`](../headerrowscount/)). Il valore massimo consentito è il limite di righe del formato file corrispondente, ad esempio per i file xlsx è 1048576. Se questa proprietà non è stata specificata o il valore specificato non è positivo, verrà utilizzato comunque il limite massimo.

### Esempi

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyMaxRowCountDemo
    {
        public static void Run()
        {
            // Crea contenuto CSV di esempio
            string content = "Header1,Header2,Header3\n" +
                            "Data1,Data2,Data3\n" +
                            "Data4,Data5,Data6\n" +
                            "Data7,Data8,Data9\n" +
                            "Data10,Data11,Data12\n" +
                            "Data13,Data14,Data15\n" +
                            "Data16,Data17,Data18";

            // Crea TxtLoadOptions con MaxRowCount impostato a 4
            TxtLoadOptions opts = new TxtLoadOptions
            {
                MaxRowCount = 4,  // Only load first 4 rows (including header)
                HeaderRowsCount = 1  // First row is header
            };

            // Carica il CSV nella cartella di lavoro
            using (MemoryStream ms = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook wb = new Workbook(ms, opts);

                // Verifica che siano state caricate solo 4 righe (1 intestazione + 3 righe di dati)
                Worksheet sheet = wb.Worksheets[0];
                Console.WriteLine($"Total rows loaded: {sheet.Cells.MaxDataRow + 1}");
                Console.WriteLine($"Row 1 (Header): {sheet.Cells[0, 0].StringValue}");
                Console.WriteLine($"Row 2 (Data): {sheet.Cells[1, 0].StringValue}");
                Console.WriteLine($"Row 3 (Data): {sheet.Cells[2, 0].StringValue}");
                Console.WriteLine($"Row 4 (Data): {sheet.Cells[3, 0].StringValue}");

                // Questo sarebbe nullo poiché abbiamo caricato solo 4 righe (indice 0-3)
                if (sheet.Cells[4, 0] == null || string.IsNullOrEmpty(sheet.Cells[4, 0].StringValue))
                {
                    Console.WriteLine("Row 5 was not loaded due to MaxRowCount limitation");
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


