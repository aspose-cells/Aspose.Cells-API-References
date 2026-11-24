---
title: "AutoFitterOptions.ForRendering"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFitterOptions-Eigenschaft. Gibt an, ob die Anpassung für Rendering-Zwecke erfolgt"
type: docs
url: /de/net/aspose.cells/autofitteroptions/forrendering/
---
## AutoFitterOptions.ForRendering property

Gibt an, ob die Anpassung für Rendering-Zwecke erfolgt.

```csharp
public bool ForRendering { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyForRenderingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit langem Text festlegen
            worksheet.Cells["A1"].PutValue("This is a long text that needs auto-fitting for rendering purposes.");
            
            // AutoFitterOptions erstellen und ForRendering auf true setzen
            AutoFitterOptions options = new AutoFitterOptions();
            options.ForRendering = true;

            // Zeile automatisch anpassen unter Berücksichtigung des Renderings
            worksheet.AutoFitRows(0, 0, options);

            // Geben Sie die resultierende Zeilenhöhe in Pixeln aus
            Console.WriteLine("Row height after auto-fitting (pixels): " + worksheet.Cells.GetRowHeightPixel(0));
        }
    }
}
```

### Siehe auch

* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


