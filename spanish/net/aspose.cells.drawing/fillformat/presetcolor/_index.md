---
title: "FillFormat.PresetColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Devuelve el color preestablecido del degradado para el relleno especificado"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/presetcolor/
---
## FillFormat.PresetColor property

Devuelve el color predefinido del degradado para el relleno especificado.

```csharp
public GradientPresetType PresetColor { get; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Acceda al formato de relleno del área del gráfico
            FillFormat fillFormat = chart.ChartArea.Area.FillFormat;

            // Establezca un color preestablecido de degradado
            fillFormat.SetPresetColorGradient(GradientPresetType.Ocean, GradientStyleType.DiagonalUp, 2);

            // Muestre y verifique el color preestablecido
            Console.WriteLine("Preset Color: " + fillFormat.PresetColor);

            // Guarda el libro de trabajo
            workbook.Save("FillFormatPresetColorDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [GradientPresetType](../../gradientpresettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


