---
title: "PageSetup.PrintHeadings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta se le intestazioni di riga e colonna vengono stampate con questa pagina"
type: docs
url: /it/net/aspose.cells/pagesetup/printheadings/
---
## PageSetup.PrintHeadings property

Rappresenta se le intestazioni di righe e colonne vengono stampate con questa pagina.

```csharp
public bool PrintHeadings { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintHeadingsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta alcuni dati di esempio con intestazioni
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);

            // Abilita la stampa delle intestazioni
            worksheet.PageSetup.PrintHeadings = true;
            worksheet.PageSetup.PrintArea = "A1:B3";

            // Salva come HTML per dimostrare l'effetto
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportActiveWorksheetOnly = true,
                ExportPrintAreaOnly = true,
                ExportGridLines = true,
                ExportHeadings = true
            };

            workbook.Save("PrintHeadingsDemo.html", saveOptions);

            Console.WriteLine("Worksheet saved with PrintHeadings enabled.");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


