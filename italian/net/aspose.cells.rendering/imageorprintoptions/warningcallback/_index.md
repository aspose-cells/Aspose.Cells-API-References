---
title: "ImageOrPrintOptions.WarningCallback"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta il callback di avviso"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/warningcallback/
---
## ImageOrPrintOptions.WarningCallback property

Ottiene o imposta il callback di avviso.

```csharp
public IWarningCallback WarningCallback { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyWarningCallbackDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi contenuto che genererà un avviso durante il rendering
            worksheet.Cells["A1"].PutValue("This text uses a non-existent font");
            Style style = workbook.CreateStyle();
            style.Font.Name = "NonExistentFont";
            worksheet.Cells["A1"].SetStyle(style);

            // Crea un'istanza di ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Visualizza il valore iniziale di WarningCallback
            Console.WriteLine("Current WarningCallback value: " + options.WarningCallback);

            // Crea e assegna un callback di avviso personalizzato
            var warningCallback = new RenderingWarningCallback();
            options.WarningCallback = warningCallback;

            // Crea SheetRender per dimostrare il callback durante il rendering
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "output_image.png");

            // Verifica se gli avvisi sono stati catturati
            Console.WriteLine($"Total warnings captured: {warningCallback.WarningCount}");
        }
    }

    // Implementazione personalizzata del callback per gestire gli avvisi di rendering
    public class RenderingWarningCallback : IWarningCallback
    {
        public int WarningCount { get; private set; }

        public void Warning(WarningInfo warningInfo)
        {
            // Gestisci gli avvisi di sostituzione dei font
            if (warningInfo.WarningType == WarningType.FontSubstitution)
            {
                Console.WriteLine($"Font substitution warning: {warningInfo.Description}");
                WarningCount++;
            }
        }
    }
}
```

### Vedi anche

* interface [IWarningCallback](../../../aspose.cells/iwarningcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


