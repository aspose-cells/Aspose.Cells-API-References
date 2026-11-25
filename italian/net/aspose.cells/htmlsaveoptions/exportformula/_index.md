---
title: "HtmlSaveOptions.ExportFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare la formula durante il salvataggio del file in html. Il valore predefinito è true. Se desideri importare l'html di output in Excel, mantieni il valore predefinito"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportformula/
---
## HtmlSaveOptions.ExportFormula property

Indica se esportare le formule quando si salva il file in html. Il valore predefinito è true. Se vuoi importare l'html di output in Excel, mantieni il valore predefinito.

```csharp
public bool ExportFormula { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportFormulaDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e formula
            worksheet.Cells["A1"].PutValue("Value 1");
            worksheet.Cells["B1"].PutValue("Value 2");
            worksheet.Cells["C1"].Formula = "=A1+B1";
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].Formula = "=A2+B2";

            // Salva con ExportFormula = true
            HtmlSaveOptions options1 = new HtmlSaveOptions();
            options1.ExportFormula = true;
            workbook.Save("output_with_formulas.html", options1);

            // Salva con ExportFormula = false
            HtmlSaveOptions options2 = new HtmlSaveOptions();
            options2.ExportFormula = false;
            workbook.Save("output_without_formulas.html", options2);

            // Verifica i risultati
            string htmlWithFormulas = File.ReadAllText("output_with_formulas.html");
            string htmlWithoutFormulas = File.ReadAllText("output_without_formulas.html");

            Console.WriteLine("HTML with formulas contains formula: " + 
                htmlWithFormulas.Contains("=A2+B2"));
            Console.WriteLine("HTML without formulas contains formula: " + 
                htmlWithoutFormulas.Contains("=A2+B2"));
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


