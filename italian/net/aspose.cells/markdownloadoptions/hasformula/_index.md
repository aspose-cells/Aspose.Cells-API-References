---
title: "MarkdownLoadOptions.HasFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MarkdownLoadOptions. Indica se il testo è una formula se inizia con"
type: docs
url: /it/net/aspose.cells/markdownloadoptions/hasformula/
---
## MarkdownLoadOptions.HasFormula property

Indica se il testo è una formula se inizia con "=\".

```csharp
public bool HasFormula { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            try
            {
                // Crea un'istanza di MarkdownLoadOptions
                MarkdownLoadOptions options = new MarkdownLoadOptions();

                // Visualizza il valore predefinito di HasFormula
                Console.WriteLine($"Default HasFormula value: {options.HasFormula}");

                // Imposta HasFormula su true
                options.HasFormula = true;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Imposta HasFormula su false
                options.HasFormula = false;
                Console.WriteLine($"HasFormula set to: {options.HasFormula}");

                // Crea una cartella di lavoro con contenuto markdown di esempio
                Workbook workbook = new Workbook();

                // Salva la cartella di lavoro per dimostrare che le opzioni possono essere usate
                workbook.Save("HasFormulaDemo.xlsx");

                Console.WriteLine("HasFormula property demonstration completed successfully.");
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

* class [MarkdownLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


