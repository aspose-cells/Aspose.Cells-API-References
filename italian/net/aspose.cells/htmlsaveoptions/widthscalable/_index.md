---
title: "HtmlSaveOptions.WidthScalable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare la larghezza della colonna in unità di scala verso HTML. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/widthscalable/
---
## HtmlSaveOptions.WidthScalable property

Indica se esportare la larghezza delle colonne in unità di scala in HTML. Il valore predefinito è false.

```csharp
public bool WidthScalable { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyWidthScalableDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con dati di test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test WidthScalable Property");
            worksheet.Cells["B1"].PutValue(123.45);
            
            // Imposta le opzioni di salvataggio HTML con la proprietà WidthScalable
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.WidthScalable = true; // Demonstrate setting to true
            
            // Salva con larghezza scalabile
            workbook.Save("output_scalable.html", options);
            
            // Salva nuovamente con larghezza fissa
            options.WidthScalable = false;
            workbook.Save("output_fixed.html", options);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


