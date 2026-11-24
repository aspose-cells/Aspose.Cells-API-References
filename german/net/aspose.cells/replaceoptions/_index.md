---
title: "Klasse ReplaceOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ReplaceOptions Klasse. Stellt die Ersetzungsoptionen dar"
type: docs
url: /de/net/aspose.cells/replaceoptions/
---
## ReplaceOptions class

Stellt die Ersetzungsoptionen dar.

```csharp
public class ReplaceOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ReplaceOptions](replaceoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CaseSensitive](../../aspose.cells/replaceoptions/casesensitive/) { get; set; } | Gibt an, ob die gesuchte Zeichenfolge Groß‑ und Kleinschreibung beachtet. |
| [FontSettings](../../aspose.cells/replaceoptions/fontsettings/) { get; set; } | Die reich formatierten Einstellungen für den ersetzten Text. |
| [MatchEntireCellContents](../../aspose.cells/replaceoptions/matchentirecellcontents/) { get; set; } | Gibt an, ob der gesamte Zelleninhalt abgeglichen werden soll. |
| [RegexKey](../../aspose.cells/replaceoptions/regexkey/) { get; set; } | Gibt an, ob der gesuchte Schlüssel ein Regex ist. Wenn true, wird der gesuchte Schlüssel als Regex behandelt. |
| [StyleFlags](../../aspose.cells/replaceoptions/styleflags/) { get; set; } | Liest und setzt Flags für die Anwendung von Schriftarteinstellungen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ReplaceOptionsDemo
    {
        public static void ReplaceOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            sheet.Cells["A1"].PutValue("Hello World");
            sheet.Cells["A2"].PutValue("Hello Aspose");
            sheet.Cells["A3"].PutValue("Goodbye World");

            // ReplaceOptions erstellen
            ReplaceOptions options = new ReplaceOptions
            {
                CaseSensitive = false,
                MatchEntireCellContents = false,
                RegexKey = false
            };

            // Ersetze "Hello" durch "Hi" im Arbeitsblatt
            int replacedCount = workbook.Replace("Hello", "Hi", options);

            // Gibt die Anzahl der vorgenommenen Ersetzungen aus
            Console.WriteLine($"Number of replacements made: {replacedCount}");

            // Speichere die Arbeitsmappe
            workbook.Save("ReplaceOptionsExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


