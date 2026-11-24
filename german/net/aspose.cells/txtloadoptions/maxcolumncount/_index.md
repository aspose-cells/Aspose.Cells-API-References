---
title: "TxtLoadOptions.MaxColumnCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtLoadOptions‑Eigenschaft. Die maximale Anzahl von Spalten, die für ein Blatt importiert werden sollen"
type: docs
url: /de/net/aspose.cells/txtloadoptions/maxcolumncount/
---
## TxtLoadOptions.MaxColumnCount property

Die maximale Anzahl von Spalten, die für ein Blatt importiert werden können.

```csharp
public int MaxColumnCount { get; set; }
```

### Hinweise

Spalten, die dieses Limit überschreiten, werden gemäß [`ExtendToNextSheet`](../extendtonextsheet/) ignoriert oder auf das nächste Blatt erweitert. Diese Anzahl schließt die Header‑Spalten ([`HeaderColumnsCount`](../headercolumnscount/)) ein. Der Maximalwert ist das Spaltenlimit des jeweiligen Dateiformats, z. B. für xlsx‑Dateien beträgt es 16384. Wenn diese Eigenschaft nicht angegeben wurde oder der angegebene Wert nicht positiv ist, wird ebenfalls das maximale Limit verwendet.

### Beispiele

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
            // Erstelle Beispiel‑CSV‑Inhalt
            string content = "A,B,C,D,E,F,G,H,I,J,K\n" +
                            "1,2,3,4,5,6,7,8,9,10,11\n" +
                            "a,b,c,d,e,f,g,h,i,j,k";

            // Erstelle TxtLoadOptions mit MaxColumnCount auf 5 gesetzt
            TxtLoadOptions options = new TxtLoadOptions
            {
                MaxColumnCount = 5  // Only load first 5 columns
            };

            // Lade die CSV mit begrenzten Spalten
            using (MemoryStream stream = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook workbook = new Workbook(stream, options);
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Gib die geladenen Daten aus (nur die ersten 5 Spalten sollten vorhanden sein)
                Console.WriteLine("Data loaded with MaxColumnCount = 5:");
                for (int row = 0; row < cells.MaxDataRow + 1; row++)
                {
                    for (int col = 0; col < cells.MaxDataColumn + 1; col++)
                    {
                        Console.Write(cells[row, col].StringValue + "\t");
                    }
                    Console.WriteLine();
                }

                // Verifiziere, dass nur 5 Spalten geladen wurden
                Console.WriteLine($"\nMax loaded columns: {cells.MaxDataColumn + 1}");
            }
        }
    }
}
```

### Siehe auch

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


