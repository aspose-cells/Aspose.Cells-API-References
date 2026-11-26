---
title: "FillFormat.SetPresetColorGradient"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FillFormat. Establece el relleno especificado a un degradado de color preestablecido. Solo se aplica a Excel 2007"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/setpresetcolorgradient/
---
## FillFormat.SetPresetColorGradient method

Establece el relleno especificado a un degradado de color predefinido. Solo se aplica a Excel 2007.

```csharp
public void SetPresetColorGradient(GradientPresetType presetColor, GradientStyleType style, 
    int variant)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| presetColor | GradientPresetType | Tipo de color preestablecido |
| estilo | GradientStyleType | Estilo de sombreado de degradado. |
| variant | Int32 | La variante del degradado. Puede ser un valor de 1 a 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetPresetColorGradientWithGradientPresetTypeGradientStylDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 5; i++)
            {
                sheet.Cells[$"A{i}"].PutValue($"Item {i-1}");
                sheet.Cells[$"B{i}"].PutValue(i * 10);
            }

            // Crear gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 8, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Aplicar relleno de degradado
            FillFormat fillFormat = chart.PlotArea.Area.FillFormat;
            fillFormat.SetPresetColorGradient(GradientPresetType.Daybreak, GradientStyleType.Vertical, 1);

            // Guarda el libro de trabajo
            workbook.Save("SetPresetColorGradientDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [GradientPresetType](../../gradientpresettype/)
* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


