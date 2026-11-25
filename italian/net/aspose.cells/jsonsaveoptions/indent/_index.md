---
title: "JsonSaveOptions.Indent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà JsonSaveOptions. Indica l'indentazione"
type: docs
url: /it/net/aspose.cells/jsonsaveoptions/indent/
---
## JsonSaveOptions.Indent property

Indica l'indentazione.

```csharp
public string Indent { get; set; }
```

### Osservazioni

Se l'indentazione è nulla o vuota, il JSON esportato non è formattato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyIndentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(25);

            // Configura le opzioni di salvataggio JSON con indentazione
            JsonSaveOptions saveOptions = new JsonSaveOptions
            {
                Indent = "    ", // 4 spaces for indentation
                ExportArea = new CellArea { StartRow = 0, EndRow = 3, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true
            };

            // Salva con output JSON indentato
            workbook.Save("IndentedJsonOutput.json", saveOptions);
        }
    }
}
```

### Vedi anche

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


