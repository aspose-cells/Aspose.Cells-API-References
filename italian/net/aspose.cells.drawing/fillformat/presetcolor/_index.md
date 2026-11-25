---
title: "FillFormat.PresetColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Restituisce il colore predefinito del gradiente per il riempimento specificato."
type: docs
url: /it/net/aspose.cells.drawing/fillformat/presetcolor/
---
## FillFormat.PresetColor property

Restituisce il colore predefinito del gradiente per il riempimento specificato.

```csharp
public GradientPresetType PresetColor { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPresetColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Accedi al formato di riempimento dell'area del grafico.
            FillFormat fillFormat = chart.ChartArea.Area.FillFormat;

            // Imposta un colore predefinito del gradiente.
            fillFormat.SetPresetColorGradient(GradientPresetType.Ocean, GradientStyleType.DiagonalUp, 2);

            // Visualizza e verifica il colore predefinito.
            Console.WriteLine("Preset Color: " + fillFormat.PresetColor);

            // Salva la cartella di lavoro
            workbook.Save("FillFormatPresetColorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [GradientPresetType](../../gradientpresettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


