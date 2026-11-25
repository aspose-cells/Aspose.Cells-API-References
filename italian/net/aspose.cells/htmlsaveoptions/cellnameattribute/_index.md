---
title: "HtmlSaveOptions.CellNameAttribute"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Specifica l'attributo che indica il CellName da scrivere. ad es. Se il valore è id, allora per la cella A1 l'output sarà td idA1. Il valore predefinito è null"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/cellnameattribute/
---
## HtmlSaveOptions.CellNameAttribute property

Specifica l'attributo che indica il CellName da scrivere. (ad esempio, se il valore è "id", allora per la cella "A1" l'output sarà:&lt;td id='A1'&gt;). Il valore predefinito è null.

```csharp
public string CellNameAttribute { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using System.Text.RegularExpressions;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCellNameAttributeDemo
    {
        public static void Run()
        {
            // Crea un workbook di esempio con alcuni dati
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["B2"].PutValue(123);

            // Imposta le opzioni di salvataggio HTML con CellNameAttribute
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellNameAttribute = "id";
            saveOptions.ExportImagesAsBase64 = true;
            saveOptions.ExportActiveWorksheetOnly = true;

            // Salva in un file HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            // Verifica che l'output HTML contenga gli ID delle celle
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains A1 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='A1'"));
            Console.WriteLine("HTML contains B2 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='B2'"));
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


