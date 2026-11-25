---
title: "LowCodeHtmlSaveOptions.HtmlOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "LowCodeHtmlSaveOptions proprietà. Le opzioni generali per il salvataggio html"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/
---
## LowCodeHtmlSaveOptions.HtmlOptions property

Le opzioni generali per il salvataggio di HTML.

```csharp
public HtmlSaveOptions HtmlOptions { get; set; }
```

### Osservazioni

Quando viene specificata un'istanza di [`HtmlSaveOptions`](../../../aspose.cells/htmlsaveoptions/), il [`SaveFormat`](../saveformat/) verrà sovrascritto (se era stato specificato in precedenza).

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeHtmlSaveOptionsPropertyHtmlOptionsDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.99);
            
            // Crea opzioni di salvataggio HTML low-code
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                SaveFormat = SaveFormat.Html,
                HtmlOptions = new HtmlSaveOptions()
            };

            // Visualizza l'impostazione corrente di esportazione delle linee della griglia
            Console.WriteLine("Export gridlines initially: " + saveOptions.HtmlOptions.ExportGridLines);

            // Salva con le linee della griglia visibili
            workbook.Save("HtmlWithGridlines.html", saveOptions.HtmlOptions);

            // Modifica le opzioni HTML per nascondere le linee della griglia
            saveOptions.HtmlOptions = new HtmlSaveOptions { ExportGridLines = false };
            Console.WriteLine("Export gridlines after modification: " + saveOptions.HtmlOptions.ExportGridLines);

            // Salva senza linee della griglia
            workbook.Save("HtmlWithoutGridlines.html", saveOptions.HtmlOptions);

            Console.WriteLine("Demo executed successfully. Compare output files.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../../../aspose.cells/htmlsaveoptions/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


