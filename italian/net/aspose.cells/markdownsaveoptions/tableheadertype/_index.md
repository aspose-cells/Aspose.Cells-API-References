---
title: "MarkdownSaveOptions.TableHeaderType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MarkdownSaveOptions. Ottiene e imposta come impostare l'intestazione della tabella"
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/tableheadertype/
---
## MarkdownSaveOptions.TableHeaderType property

Ottiene e imposta come impostare l'intestazione della tabella.

```csharp
public MarkdownTableHeaderType TableHeaderType { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per creare una tabella
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Crea MarkdownSaveOptions e imposta TableHeaderType
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;

            // Salva come markdown con le opzioni specificate
            workbook.Save("output.md", saveOptions);
        }
    }
}
```

### Vedi anche

* enum [MarkdownTableHeaderType](../../../aspose.cells.markdown/markdowntableheadertype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


