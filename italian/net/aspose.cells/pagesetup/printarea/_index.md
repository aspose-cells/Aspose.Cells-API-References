---
title: "PageSetup.PrintArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PageSetup. Rappresenta l'intervallo da stampare"
type: docs
url: /it/net/aspose.cells/pagesetup/printarea/
---
## PageSetup.PrintArea property

Rappresenta l'intervallo da stampare.

```csharp
public string PrintArea { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(3);
            
            // Imposta l'area di stampa su A1:B3
            worksheet.PageSetup.PrintArea = "A1:B3";
            
            // Salva solo con l'area di stampa
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportPrintAreaOnly = true
            };
            
            workbook.Save("PrintAreaDemo.html", options);
            
            Console.WriteLine("Print area demo created successfully.");
        }
    }
}
```

### Vedi anche

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


