---
title: "TxtLoadOptions.MaxColumnCount"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtLoadOptions. Il numero massimo di colonne da importare per un foglio"
type: docs
url: /it/net/aspose.cells/txtloadoptions/maxcolumncount/
---
## TxtLoadOptions.MaxColumnCount property

Il conteggio massimo di colonne da importare per un foglio.

```csharp
public int MaxColumnCount { get; set; }
```

### Osservazioni

Le colonne che superano questo limite verranno ignorate o estese al foglio successivo secondo [`ExtendToNextSheet`](../extendtonextsheet/). Questo conteggio include le colonne di intestazione ([`HeaderColumnsCount`](../headercolumnscount/)). Il valore massimo è il limite di colonne del formato file corrispondente, ad esempio per i file xlsx è 16384. Se questa proprietà non è stata specificata o il valore specificato non è positivo, verrà comunque utilizzato il limite massimo.

### Esempi

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
            // Crea contenuto CSV di esempio
            string content = "A,B,C,D,E,F,G,H,I,J,K\n" +
                            "1,2,3,4,5,6,7,8,9,10,11\n" +
                            "a,b,c,d,e,f,g,h,i,j,k";

            // Crea TxtLoadOptions con MaxColumnCount impostato a 5
            TxtLoadOptions options = new TxtLoadOptions
            {
                MaxColumnCount = 5  // Only load first 5 columns
            };

            // Carica il CSV con colonne limitate
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Visualizza i dati caricati (dovrebbero essere presenti solo le prime 5 colonne)
                Console.WriteLine("Data loaded with MaxColumnCount = 5:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // Verifica che siano state caricate solo 5 colonne
                Console.WriteLine($"\nMax loaded columns: {cells.MaxDataColumn + 1}");
            }
        }
    }
}
```

### Vedi anche

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


