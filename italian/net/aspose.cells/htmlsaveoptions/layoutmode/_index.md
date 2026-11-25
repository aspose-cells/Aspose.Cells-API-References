---
title: "HtmlSaveOptions.LayoutMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Ottiene o imposta la modalità di layout durante il salvataggio in HTML. Il valore predefinito è Normal"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/layoutmode/
---
## HtmlSaveOptions.LayoutMode property

Ottiene o imposta la modalità di layout quando si salva in HTML. Il valore predefinito è Normal

```csharp
public HtmlLayoutMode LayoutMode { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyLayoutModeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Layout Mode Test");

            try
            {
                // Crea un'istanza di HtmlSaveOptions
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Visualizza il valore corrente di LayoutMode
                Console.WriteLine("Current LayoutMode: " + options.LayoutMode);

                // Imposta LayoutMode su Print
                options.LayoutMode = HtmlLayoutMode.Print;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Salva la cartella di lavoro con modalità di layout Print
                workbook.Save("LayoutModePrint.html", options);

                // Imposta LayoutMode su Normal
                options.LayoutMode = HtmlLayoutMode.Normal;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Salva la cartella di lavoro con modalità di layout Normal
                workbook.Save("LayoutModeNormal.html", options);

                Console.WriteLine("HTML files saved with different LayoutMode settings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [HtmlLayoutMode](../../../aspose.cells.rendering/htmllayoutmode/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


