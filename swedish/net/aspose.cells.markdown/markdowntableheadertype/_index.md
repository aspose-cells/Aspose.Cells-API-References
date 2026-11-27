---
title: "Enum MarkdownTableHeaderType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Markdown.MarkdownTableHeaderType enum. Representerar rubriktypen för tabellen i markdown‑filen."
type: docs
url: /sv/net/aspose.cells.markdown/markdowntableheadertype/
---
## MarkdownTableHeaderType enumeration

Representerar rubriktypen för tabellen i markdown-filen.

```csharp
public enum MarkdownTableHeaderType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| FirstRow | `0` | Första raden som rubrik i tabellen. |
| ColumnHeader | `1` | Kolumnnamn (såsom A,B,C...) som rubrik i tabellen. |
| Empty | `2` | En tom rubrikrad. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Ställ in Markdown‑sparalternativ
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // Spara som Markdown‑fil
            workbook.Save("output.md", saveOptions);
            
            // Verifiera resultatet
            string text = File.ReadAllText("output.md");
            Console.WriteLine(text.Contains("---|") ? "Success" : "Failed");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Markdown](../../aspose.cells.markdown/)
* assembly [Aspose.Cells](../../)


