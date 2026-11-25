---
title: "MarkdownSaveOptions.OfficeMathOutputType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MarkdownSaveOptions. Indica come gli oggetti OfficeMath vengono esportati in Markdown. Il valore predefinito è Image"
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/officemathoutputtype/
---
## MarkdownSaveOptions.OfficeMathOutputType property

Indica come gli oggetti OfficeMath vengono esportati in Markdown, il valore predefinito è Image.

```csharp
public HtmlOfficeMathOutputType OfficeMathOutputType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio includendo una formula che potrebbe contenere OfficeMath
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].Formula = "=SQRT(16)";

            try
            {
                // Crea le opzioni di salvataggio Markdown
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Visualizza il valore corrente di OfficeMathOutputType
                Console.WriteLine("Current OfficeMathOutputType: " + saveOptions.OfficeMathOutputType);

                // Imposta OfficeMathOutputType su MathML
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.MathML;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // Salva la cartella di lavoro con il tipo di output MathML
                workbook.Save("OfficeMathOutputType_MathML.md", saveOptions);

                // Cambia al tipo di output Image
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.Image;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // Salva la cartella di lavoro con il tipo di output Image
                workbook.Save("OfficeMathOutputType_Image.md", saveOptions);

                Console.WriteLine("OfficeMathOutputType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [HtmlOfficeMathOutputType](../../htmlofficemathoutputtype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


