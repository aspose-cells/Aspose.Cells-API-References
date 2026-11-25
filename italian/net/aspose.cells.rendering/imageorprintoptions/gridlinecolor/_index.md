---
title: "ImageOrPrintOptions.GridlineColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ImageOrPrintOptions property. Ottiene o imposta il colore della griglia"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/gridlinecolor/
---
## ImageOrPrintOptions.GridlineColor property

Ottiene o imposta il colore della griglia.

```csharp
public Color GridlineColor { get; set; }
```

### Osservazioni

Ignorerà le impostazioni del colore della linea della griglia nel file di origine.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci alcuni dati di esempio in modo che il foglio di lavoro abbia contenuto
            worksheet.Cells["A1"].PutValue("Demo for GridlineColor property");

            try
            {
                // Crea un'istanza di ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Visualizza il valore corrente di GridlineColor (sola lettura o lettura/scrittura)
                // Il tipo della proprietà è presumibilmente System.Drawing.Color
                Console.WriteLine("Current GridlineColor: " + options.GridlineColor);

                // Facoltativamente esegui il rendering del foglio in un'immagine per vedere l'effetto del colore della griglia predefinito
                // (Non è necessario modificare il valore; dimostriamo solo l'uso.)
                SheetRender renderer = new SheetRender(worksheet, options);
                renderer.ToImage(0, "GridlineColorDemo.png");

                // Salva la cartella di lavoro (opzionale)
                workbook.Save("GridlineColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during demo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


