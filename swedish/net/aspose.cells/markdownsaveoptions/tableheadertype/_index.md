---
title: "MarkdownSaveOptions.TableHeaderType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions‑egenskap. Hämtar och anger hur tabellens rubrik ska sättas"
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/tableheadertype/
---
## MarkdownSaveOptions.TableHeaderType property

Hämtar och anger hur tabellens rubrik ska sättas.

```csharp
public MarkdownTableHeaderType TableHeaderType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markdown;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyTableHeaderTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att skapa en tabell
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Skapa MarkdownSaveOptions och ange TableHeaderType
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;

            // Spara som markdown med angivna alternativ
            workbook.Save("output.md", saveOptions);
        }
    }
}
```

### Se även

* enum [MarkdownTableHeaderType](../../../aspose.cells.markdown/markdowntableheadertype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


