---
title: "HtmlSaveOptions.MergeEmptyTdForcely"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se unire forzatamente gli elementi TD vuoti durante l'esportazione del file in html. La dimensione del file html sarà ridotta significativamente impostando il valore su true. Il valore predefinito è false. Se desideri importare il file html in Excel o esportare linee di griglia perfette quando salvi il file in html, mantieni il valore predefinito."
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/mergeemptytdforcely/
---
## HtmlSaveOptions.MergeEmptyTdForcely property

Indica se unire forzatamente gli elementi TD vuoti durante l'esportazione del file in html. La dimensione del file html sarà ridotta significativamente impostando il valore su true. Il valore predefinito è false. Se desideri importare il file html in Excel o esportare linee di griglia perfette quando salvi il file in html, mantieni il valore predefinito.

```csharp
[Obsolete("Use HtmlSaveOptions.MergeEmptyTdType instead.")]
public bool MergeEmptyTdForcely { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyMergeEmptyTdForcelyDemo
    {
        public static void Run()
        {
            // Crea un workbook di esempio con celle vuote
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea alcune celle vuote nel foglio di lavoro
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            // B2 è lasciato intenzionalmente vuoto
            
            // Salva con MergeEmptyTdForcely abilitato
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.MergeEmptyTdForcely = true;
            workbook.Save("output_with_merge.html", options);
            
            // Salva senza MergeEmptyTdForcely per confronto
            options.MergeEmptyTdForcely = false;
            workbook.Save("output_without_merge.html", options);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


