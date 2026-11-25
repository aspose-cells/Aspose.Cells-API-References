---
title: "HtmlLoadOptions.ConvertFormulasData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlLoadOptions. se true converte la stringa in formula quando il valore della stringa inizia con il carattere, il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlloadoptions/convertformulasdata/
---
## HtmlLoadOptions.ConvertFormulasData property

se true, converte la stringa in formula quando il valore della stringa inizia con il carattere '=', il valore predefinito è false.

```csharp
[Obsolete("Use HtmlLoadOptions.HasFormula property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ConvertFormulasData { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà HtmlLoadOptions.HasFormula. Questa proprietà sarà rimossa 12 mesi dopo, a partire da marzo 2023. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyConvertFormulasDataDemo
    {
        public static void Run()
        {
            // Crea un'istanza di HtmlLoadOptions
            HtmlLoadOptions options = new HtmlLoadOptions();

            // Imposta la proprietà ConvertFormulasData su true
            options.ConvertFormulasData = true;

            // Carica un file HTML in una cartella di lavoro utilizzando le opzioni specificate
            Workbook workbook = new Workbook("input.html", options);

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Visualizza alcuni valori di cella per dimostrare la conversione delle formule
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell B1 formula: " + worksheet.Cells["B1"].Formula);

            // Salva la cartella di lavoro in un file Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


