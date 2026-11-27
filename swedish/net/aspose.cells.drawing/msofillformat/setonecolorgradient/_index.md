---
title: "MsoFillFormat.SetOneColorGradient"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFillFormat method. Anger den specificerade fyllningen till en enfärgsgradient"
type: docs
url: /sv/net/aspose.cells.drawing/msofillformat/setonecolorgradient/
---
## MsoFillFormat.SetOneColorGradient method

Ställer in den angivna fyllningen till en enfärgsgradient.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| färg | Färg | En gradientfärg. |
| grad | Double | Gradientens grad. Kan vara ett värde från 0,0 (mörk) till 1,0 (ljus). |
| style | GradientStyleType | Gradientskuggningsstil. |
| variant | Int32 | Gradientvarianten. Kan vara ett värde från 1 till 4, motsvarande en av de fyra varianterna på fliken Gradient i dialogrutan Fylleffekter. Om stil är GradientStyle.FromCenter, kan Variant‑argumentet endast vara 1 eller 2. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatMethodSetOneColorGradientWithColorDoubleGradientStyleTypeInDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 50, 50);
            MsoFillFormat fillFormat = shape.FillFormat;

            // Ställ in enfärgsgradient med specificerade parametrar
            fillFormat.SetOneColorGradient(Color.Red, 0.5, GradientStyleType.DiagonalUp, 2);

            workbook.Save("GradientFillExample.xlsx");
        }
    }
}
```

### Se även

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


