---
title: "MarkdownSaveOptions.FormatStrategy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MarkdownSaveOptions. Ottiene e imposta la strategia di formattazione quando si esporta il valore della cella come stringa"
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/formatstrategy/
---
## MarkdownSaveOptions.FormatStrategy property

Ottiene e imposta la strategia di formattazione quando si esporta il valore della cella come stringa.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Esempi

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con formati diversi
            worksheet.Cells["A1"].PutValue(123.456); // Numeric value
            worksheet.Cells["A2"].PutValue(DateTime.Now); // Date value
            worksheet.Cells["A3"].PutValue(true); // Boolean value

            // Crea le opzioni di salvataggio Markdown con la strategia di formattazione DisplayString
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayString
            };

            // Salva la cartella di lavoro come Markdown
            workbook.Save("MarkdownWithDisplayString.md", saveOptions);

            // Cambia a CellValueFormatStrategy.CellStyle
            saveOptions.FormatStrategy = CellValueFormatStrategy.CellStyle;
            workbook.Save("MarkdownWithCellStyle.md", saveOptions);

            Console.WriteLine("Markdown files saved successfully with different format strategies.");
        }
    }
}
```

### Vedi anche

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


