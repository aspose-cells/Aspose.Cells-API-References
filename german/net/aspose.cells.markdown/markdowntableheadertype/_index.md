---
title: "Aufzählung MarkdownTableHeaderType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Markdown.MarkdownTableHeaderType Enum. Gibt den Header‑Typ der Tabelle in der Markdown‑Datei an."
type: docs
url: /de/net/aspose.cells.markdown/markdowntableheadertype/
---
## MarkdownTableHeaderType enumeration

Stellt den Header-Typ der Tabelle in der Markdown-Datei dar.

```csharp
public enum MarkdownTableHeaderType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| FirstRow | `0` | Erste Zeile als Header der Tabelle. |
| ColumnHeader | `1` | Spaltenname (wie A,B,C…) als Header der Tabelle. |
| Empty | `2` | Eine leere Header‑Zeile. |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Markdown;

namespace AsposeCellsExamples
{
    public class MarkdownClassMarkdownTableHeaderTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Markdown‑Speicheroptionen festlegen
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // Als Markdown‑Datei speichern
            workbook.Save("output.md", saveOptions);
            
            // Ausgabe überprüfen
            string text = File.ReadAllText("output.md");
            Console.WriteLine(text.Contains("---|") ? "Success" : "Failed");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Markdown](../../aspose.cells.markdown/)
* assembly [Aspose.Cells](../../)


