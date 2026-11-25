---
title: "LoadOptions.IgnoreNotPrinted"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Ignora i dati che non sono stampati se si stampa direttamente il file"
type: docs
url: /it/net/aspose.cells/loadoptions/ignorenotprinted/
---
## LoadOptions.IgnoreNotPrinted property

Ignora i dati che non vengono stampati se si stampa direttamente il file

```csharp
public bool IgnoreNotPrinted { get; set; }
```

### Osservazioni

Solo per file xlsx.

### Esempi

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreNotPrintedDemo
    {
        public static void Run()
        {
            // Crea opzioni di caricamento HTML e imposta IgnoreNotPrinted
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.AutoFitColsAndRows = true;

            // Carica il file HTML con le opzioni specificate
            Workbook workbook = new Workbook("example.html", loadOptions);
            Worksheet worksheet = workbook.Worksheets[0];

            // Dimostra l'effetto di IgnoreNotPrinted controllando gli stili delle celle
            Console.WriteLine("B3 Cell Color: " + worksheet.Cells["B3"].GetStyle().ForegroundColor);
            Console.WriteLine("B4 Cell Color: " + worksheet.Cells["B4"].GetStyle().ForegroundColor);
            Console.WriteLine("B5 Cell Color: " + worksheet.Cells["B5"].GetStyle().ForegroundColor);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


