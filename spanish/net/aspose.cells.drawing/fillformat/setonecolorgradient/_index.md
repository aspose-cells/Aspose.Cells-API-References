---
title: "FillFormat.SetOneColorGradient"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FillFormat. Establece el relleno especificado a un degradado de un solo color. Solo se aplica a Excel 2007"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/setonecolorgradient/
---
## FillFormat.SetOneColorGradient method

Establece el relleno especificado a un degradado de un color. Solo se aplica a Excel 2007.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color | Color | Un color de degradado. |
| grado | Double | El grado del degradado. Puede ser un valor de 0.0 (oscuro) a 1.0 (claro). |
| estilo | GradientStyleType | Estilo de sombreado de degradado. |
| variant | Int32 | La variante del degradado. Puede ser un valor de 1 a 4, correspondiente a una de las cuatro variantes en la pestaña Degradado del cuadro de diálogo Efectos de relleno. Si el estilo es GradientStyle.FromCenter, el argumento Variant solo puede ser 1 o 2. |

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetOneColorGradientWithColorDoubleGradientStyleTypeInDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Values");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aplicar relleno de degradado a la primera serie
            Series series = chart.NSeries[0];
            series.IsColorVaried = false;
            
            // Demuestra SetOneColorGradient con parámetros específicos
            series.Area.FillFormat.SetOneColorGradient(
                Color.FromArgb(0, 236, 102, 102), // Color
                0.9,                              // Transparency
                Aspose.Cells.Drawing.GradientStyleType.DiagonalDown,    // Gradient style
                2);                                // Variant

            // Guarda el libro de trabajo
            workbook.Save("FillFormat_SetOneColorGradient_Output.xlsx");
        }
    }
}
```

### Ver también

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


