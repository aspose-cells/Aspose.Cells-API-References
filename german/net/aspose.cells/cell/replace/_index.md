---
title: "Cell.Replace"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell‑Methode. Ersetzt den Text der Zelle mit Optionen"
type: docs
url: /de/net/aspose.cells/cell/replace/
---
## Cell.Replace method

Text der Zelle mit Optionen ersetzen.

```csharp
public void Replace(string placeHolder, string newValue, ReplaceOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Platzhalter | String | Zellen-Platzhalter |
| newValue | String | String-Wert zum Ersetzen |
| Optionen | ReplaceOptions | Die Ersetzungsoptionen |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodReplaceWithStringStringReplaceOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("hello world");
            worksheet.Cells["A3"].PutValue("HELLO WORLD");
            worksheet.Cells["B1"].PutValue("Replaced");

            // Erstelle Ersetzungsoptionen
            ReplaceOptions options = new ReplaceOptions();
            options.CaseSensitive = false;
            options.MatchEntireCellContents = false;

            // Hole Schriftarteinstellungen aus Zelle B1, um sie auf Ersetzungen anzuwenden
            options.FontSettings = worksheet.Cells["B1"].GetCharacters();

            // Ersetze alle Varianten von "hello" durch "Hi" unter Verwendung der Optionen
            foreach (Cell cell in worksheet.Cells)
            {
                cell.Replace("Hello", "Hi", options);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [ReplaceOptions](../../replaceoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


