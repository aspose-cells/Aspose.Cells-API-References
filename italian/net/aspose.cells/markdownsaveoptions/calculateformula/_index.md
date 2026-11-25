---
title: "MarkdownSaveOptions.CalculateFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "MarkdownSaveOptions proprietà. Indica se calcolare le formule prima di salvare il file markdown"
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/calculateformula/
---
## MarkdownSaveOptions.CalculateFormula property

Indica se calcolare le formule prima di salvare il file markdown.

```csharp
public bool CalculateFormula { get; set; }
```

### Osservazioni

Il valore predefinito è false.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con formule
            worksheet.Cells["A1"].PutValue("Price");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["C1"].PutValue("Total");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["C2"].Formula = "=A2*B2";

            try
            {
                // Crea un'istanza di MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Visualizza il valore predefinito di CalculateFormula
                Console.WriteLine("Default CalculateFormula value: " + saveOptions.CalculateFormula);

                // Imposta CalculateFormula su true per calcolare le formule prima del salvataggio
                saveOptions.CalculateFormula = true;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Salva la cartella di lavoro con il calcolo delle formule abilitato
                workbook.Save("CalculateFormula_Enabled.md", saveOptions);

                // Imposta CalculateFormula su false per salvare le formule così come sono
                saveOptions.CalculateFormula = false;
                Console.WriteLine("CalculateFormula set to: " + saveOptions.CalculateFormula);

                // Salva la cartella di lavoro con il calcolo delle formule disabilitato
                workbook.Save("CalculateFormula_Disabled.md", saveOptions);

                Console.WriteLine("CalculateFormula demonstration completed successfully.");
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

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


