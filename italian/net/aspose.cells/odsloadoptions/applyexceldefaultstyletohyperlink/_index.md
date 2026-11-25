---
title: "OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OdsLoadOptions. Indica se applicare lo stile predefinito di Excel al collegamento ipertestuale"
type: docs
url: /it/net/aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink/
---
## OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink property

Indica se applicare lo stile predefinito di Excel al collegamento ipertestuale.

```csharp
public bool ApplyExcelDefaultStyleToHyperlink { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsPropertyApplyExcelDefaultStyleToHyperlinkDemo
    {
        public static void Run()
        {
            // Crea un'istanza di OdsLoadOptions
            OdsLoadOptions loadOptions = new OdsLoadOptions();

            // Imposta la proprietà ApplyExcelDefaultStyleToHyperlink
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            // Carica un file ODS con le opzioni specificate
            Workbook workbook = new Workbook("sample.ods", loadOptions);

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un collegamento ipertestuale per dimostrare l'applicazione dello stile
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Salva la cartella di lavoro in un nuovo file
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


