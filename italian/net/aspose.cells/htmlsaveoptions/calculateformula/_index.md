---
title: "HtmlSaveOptions.CalculateFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se calcolare le formule prima di salvare il file HTML"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/calculateformula/
---
## HtmlSaveOptions.CalculateFormula property

Indica se calcolare le formule prima di salvare il file html.

```csharp
public bool CalculateFormula { get; set; }
```

### Osservazioni

Il valore predefinito è false.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCalculateFormulaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati e formule al foglio di lavoro
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Crea HtmlSaveOptions con CalculateFormula impostato su true
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                CalculateFormula = true
            };

            // Salva la cartella di lavoro come HTML - le formule saranno calcolate
            workbook.Save("HtmlWithCalculatedFormulas.html", saveOptions);

            Console.WriteLine("HTML file with calculated formulas created successfully.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


