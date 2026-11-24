---
title: "TxtLoadOptions.PreferredParsers"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtLoadOptions-Eigenschaft. Ruft bevorzugte Wertparser für das Laden von Textdateien ab und legt sie fest"
type: docs
url: /de/net/aspose.cells/txtloadoptions/preferredparsers/
---
## TxtLoadOptions.PreferredParsers property

Liest und setzt bevorzugte Wertparser zum Laden einer Textdatei.

```csharp
public ICustomParser[] PreferredParsers { get; set; }
```

### Hinweise

parsers[0] ist der Parser, der für die erste Spalte in der Textvorlagendatei verwendet wird, parsers[1] ist der Parser, der für die zweite Spalte verwendet wird, … usw. Der letzte (parsers[parsers.length-1]) wird für alle anderen Spalten ab parsers.length-1 verwendet. Wenn ein Element null ist, wird die entsprechende Spalte vom Standard‑Parser von Aspose.Cells geparst.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertyPreferredParsersDemo
    {
        private class StringParser : ICustomParser
        {
            public bool Parse(string value, out object result)
            {
                result = value; // Always return as string
                return true;
            }

            public object ParseObject(string value)
            {
                return value; // Always return as string
            }

            public string GetFormat()
            {
                return "String"; // Return format description
            }
        }

        public static void Run()
        {
            // CSV-Ladeoptionen erstellen
            TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
            
            // Setze bevorzugte Parser – zuerst benutzerdefinierten String‑Parser versuchen, dann Standard‑Parser
            options.PreferredParsers = new ICustomParser[] { new StringParser(), null };

            // Beispieldaten im CSV-Format mit Datumsangaben
            string csvData = "\"2018-10-08\",2018-10-08\n\"2018-10-08\",2018-10-08";
            
            // Arbeitsmappe mit Optionen laden
            Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
            Cells cells = workbook.Worksheets[0].Cells;

            // Überprüfe die Parsergebnisse
            Console.WriteLine("A1 Type: " + cells[0, 0].Type); // Should be string
            Console.WriteLine("A1 Value: " + cells[0, 0].StringValue); // "2018-10-08"
            Console.WriteLine("B1 Type: " + cells[0, 1].Type); // Should be DateTime
            Console.WriteLine("B1 Value: " + cells[0, 1].DateTimeValue); // 10/8/2018
        }
    }
}
```

### Siehe auch

* interface [ICustomParser](../../icustomparser/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


