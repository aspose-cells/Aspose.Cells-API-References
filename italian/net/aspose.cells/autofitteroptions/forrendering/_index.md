---
title: "AutoFitterOptions.ForRendering"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AutoFitterOptions. Indica se adattare per scopi di rendering"
type: docs
url: /it/net/aspose.cells/autofitteroptions/forrendering/
---
## AutoFitterOptions.ForRendering property

Indica se adattare per scopi di rendering.

```csharp
public bool ForRendering { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyForRenderingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta dati di esempio con testo lungo
            worksheet.Cells["A1"].PutValue("This is a long text that needs auto-fitting for rendering purposes.");
            
            // Crea AutoFitterOptions e imposta ForRendering a true
            AutoFitterOptions options = new AutoFitterOptions();
            options.ForRendering = true;

            // Adatta automaticamente la riga tenendo conto del rendering
            worksheet.AutoFitRows(0, 0, options);

            // Restituisci l'altezza risultante della riga in pixel
            Console.WriteLine("Row height after auto-fitting (pixels): " + worksheet.Cells.GetRowHeightPixel(0));
        }
    }
}
```

### Vedi anche

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


