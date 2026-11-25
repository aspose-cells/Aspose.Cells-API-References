---
title: "Enum HtmlLayoutMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Rendering.HtmlLayoutMode. Rappresenta la modalità di layout per il rendering HTML"
type: docs
url: /it/net/aspose.cells.rendering/htmllayoutmode/
---
## HtmlLayoutMode enumeration

Rappresenta la modalità di layout per il rendering HTML.

```csharp
public enum HtmlLayoutMode
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Normal | `0` | Esegue il rendering del contenuto come MS Excel. |
| Print | `1` | Esegue il rendering del contenuto in modalità layout di stampa. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassHtmlLayoutModeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi alcuni dati di esempio al foglio di lavoro
                worksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");
                worksheet.Cells["A2"].PutValue("This demonstrates HtmlLayoutMode");

                // Crea HtmlSaveOptions e imposta la modalità di layout su Normal
                HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                saveOptions.LayoutMode = HtmlLayoutMode.Normal;

                // Salva la cartella di lavoro con modalità di layout normale
                workbook.Save("NormalLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Normal layout mode.");

                // Cambia la modalità di layout su Print
                saveOptions.LayoutMode = HtmlLayoutMode.Print;

                // Salva la cartella di lavoro con modalità di layout di stampa
                workbook.Save("PrintLayoutDemo.html", saveOptions);
                Console.WriteLine("Workbook saved with Print layout mode.");

                // Visualizzare i valori dell'enumerazione
                Console.WriteLine($"Normal mode value: {HtmlLayoutMode.Normal}");
                Console.WriteLine($"Print mode value: {HtmlLayoutMode.Print}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with HtmlLayoutMode: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


