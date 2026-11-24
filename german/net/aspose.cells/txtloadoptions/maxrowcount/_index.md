---
title: "TxtLoadOptions.MaxRowCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtLoadOptions‑Eigenschaft. Die maximale Anzahl von Zeilen, die für ein Blatt importiert werden sollen"
type: docs
url: /de/net/aspose.cells/txtloadoptions/maxrowcount/
---
## TxtLoadOptions.MaxRowCount property

Die maximale Anzahl von Zeilen, die für ein Blatt importiert werden können.

```csharp
public int MaxRowCount { get; set; }
```

### Hinweise

Zeilen, die dieses Limit überschreiten, werden ignoriert oder gemäß [`ExtendToNextSheet`](../extendtonextsheet/) auf das nächste Blatt erweitert. Diese Anzahl beinhaltet die Kopfzeilen ([`HeaderRowsCount`](../headerrowscount/)). Der maximal zulässige Wert ist das Zeilenlimit des jeweiligen Dateiformats, zum Beispiel für xlsx‑Dateien 1048576. Wenn diese Eigenschaft nicht angegeben wurde oder der angegebene Wert nicht positiv ist, wird ebenfalls das maximale Limit verwendet.

### Beispiele

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
            // Erstelle Beispiel‑CSV‑Inhalt
            string content = "Header1,Header2,Header3\n" +
                            "Data1,Data2,Data3\n" +
                            "Data4,Data5,Data6\n" +
                            "Data7,Data8,Data9\n" +
                            "Data10,Data11,Data12\n" +
                            "Data13,Data14,Data15\n" +
                            "Data16,Data17,Data18";

            // Erstelle TxtLoadOptions mit MaxRowCount auf 4 gesetzt
            TxtLoadOptions opts = new TxtLoadOptions
            {
                MaxRowCount = 4,  // Only load first 4 rows (including header)
                HeaderRowsCount = 1  // First row is header
            };

            // Lade die CSV in die Arbeitsmappe
            using (MemoryStream ms = new MemoryStream(Encoding.UTF8.GetBytes(content)))
            {
                Workbook wb = new Workbook(ms, opts);

                // Verifiziere, dass nur 4 Zeilen geladen wurden (1 Kopfzeile + 3 Datenzeilen)
                Worksheet sheet = wb.Worksheets[0];
                Console.WriteLine($"Total rows loaded: {sheet.Cells.MaxDataRow + 1}");
                Console.WriteLine($"Row 1 (Header): {sheet.Cells[0, 0].StringValue}");
                Console.WriteLine($"Row 2 (Data): {sheet.Cells[1, 0].StringValue}");
                Console.WriteLine($"Row 3 (Data): {sheet.Cells[2, 0].StringValue}");
                Console.WriteLine($"Row 4 (Data): {sheet.Cells[3, 0].StringValue}");

                // Dies wäre null, da wir nur 4 Zeilen geladen haben (Index 0‑3)
                if (sheet.Cells[4, 0] == null || string.IsNullOrEmpty(sheet.Cells[4, 0].StringValue))
                {
                    Console.WriteLine("Row 5 was not loaded due to MaxRowCount limitation");
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


