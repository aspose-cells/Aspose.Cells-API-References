---
title: "FillFormat.PresetColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Returnerar den förinställda gradientfärgen för den angivna fyllningen"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/presetcolor/
---
## FillFormat.PresetColor property

Returnerar den förinställda gradientfärgen för den angivna fyllningen.

```csharp
public GradientPresetType PresetColor { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Åtkomst till fyllningsformatet för diagramområdet
            FillFormat fillFormat = chart.ChartArea.Area.FillFormat;

            // Ange en förinställd gradientfärg
            fillFormat.SetPresetColorGradient(GradientPresetType.Ocean, GradientStyleType.DiagonalUp, 2);

            // Visa och verifiera den förinställda färgen
            Console.WriteLine("Preset Color: " + fillFormat.PresetColor);

            // Spara arbetsboken
            workbook.Save("FillFormatPresetColorDemo.xlsx");
        }
    }
}
```

### Se även

* enum [GradientPresetType](../../gradientpresettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


