---
title: "LoadOptions.CultureInfo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Ottiene o imposta le impostazioni regionali utilizzate per il Workbook che verrà caricato"
type: docs
url: /it/net/aspose.cells/loadoptions/cultureinfo/
---
## LoadOptions.CultureInfo property

Ottiene o imposta le impostazioni regionali utilizzate per il Workbook che verrà caricato.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Osservazioni

Questa proprietà ha lo stesso effetto di [`Region`](../region/) per impostare le impostazioni regionali.

### Esempi

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCultureInfoDemo
    {
        public static void Run()
        {
            // Crea un file Excel di esempio
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].PutValue(1234.56);
            sampleWorkbook.Save("sample.xlsx", SaveFormat.Xlsx);

            // Carica con una cultura specifica
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CultureInfo = new CultureInfo("de-DE"); // German culture uses comma as decimal separator
            
            Workbook workbook = new Workbook("sample.xlsx", options);
            Console.WriteLine("Value with German culture: " + workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


