---
title: "ExportRangeToJsonOptions.Indent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExportRangeToJsonOptions. Indica l'indentazione"
type: docs
url: /it/net/aspose.cells.utility/exportrangetojsonoptions/indent/
---
## ExportRangeToJsonOptions.Indent property

Indica l'indentazione.

```csharp
public string Indent { get; set; }
```

### Osservazioni

Se l'indentazione è nulla o vuota, il JSON esportato non è formattato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyIndentDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea un'istanza di ExportRangeToJsonOptions
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.HasHeaderRow = true;

            // Mostra l'indentazione corrente (il valore predefinito è null)
            Console.WriteLine("Current Indent value: " + (options.Indent ?? "null"));

            // Esporta con indentazione predefinita (JSON compatto)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B3");
            string jsonWithoutIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without indent:\n" + jsonWithoutIndent);

            // Imposta l'indentazione a 4 spazi
            options.Indent = "    ";
            string jsonWithIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("\nJSON with 4-space indent:\n" + jsonWithIndent);

            // Imposta l'indentazione al carattere di tabulazione
            options.Indent = "\t";
            string jsonWithTabIndent = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("\nJSON with tab indent:\n" + jsonWithTabIndent);
        }
    }
}
```

### Vedi anche

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


