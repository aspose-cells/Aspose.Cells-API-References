---
title: "ReplaceOptions.RegexKey"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ReplaceOptions-Eigenschaft. Gibt an, ob der gesuchte Schlüssel ein Regex ist. Wenn true, wird der gesuchte Schlüssel als Regex behandelt"
type: docs
url: /de/net/aspose.cells/replaceoptions/regexkey/
---
## ReplaceOptions.RegexKey property

Gibt an, ob der gesuchte Schlüssel ein Regex ist. Wenn true, wird der gesuchte Schlüssel als Regex behandelt.

```csharp
public bool RegexKey { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReplaceOptionsPropertyRegexKeyDemo
    {
        public static void Run()
        {
            // Arbeitsmappe mit Beispieldaten erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("apple");
            worksheet.Cells["A2"].PutValue("banana");
            worksheet.Cells["A3"].PutValue("orange");
            worksheet.Cells["A4"].PutValue("pear");
            worksheet.Cells["A5"].PutValue("plum");

            // Ersetzen-Optionen mit Regex erstellen
            ReplaceOptions options = new ReplaceOptions();
            options.RegexKey = true; // Enable regex matching
            
            // Alle Wörter ersetzen, die mit 'p' oder 'b' beginnen, gefolgt von einem Vokal
            string pattern = "^[pb][aeiou]";
            string replacement = "FRUIT";
            
            // Ersetzung ausführen
            workbook.Replace(pattern, replacement, options);

            // Ergebnis speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


