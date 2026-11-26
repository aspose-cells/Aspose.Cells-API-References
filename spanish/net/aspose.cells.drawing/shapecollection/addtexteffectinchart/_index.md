---
title: "ShapeCollection.AddTextEffectInChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ShapeCollection método. Inserta un objeto WordArt en el gráfico"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addtexteffectinchart/
---
## ShapeCollection.AddTextEffectInChart method

Inserta un objeto WordArt al gráfico.

```csharp
public Shape AddTextEffectInChart(MsoPresetTextEffect effect, string text, string fontName, 
    int size, bool fontBold, bool fontItalic, int top, int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| efecto | MsoPresetTextEffect | El tipo de efecto de texto predefinido mso. |
| texto | String | El texto WordArt. |
| fontName | String | El nombre de la fuente. |
| tamaño | Int32 | El tamaño de la fuente |
| fontBold | Booleano | Indica si la fuente está en negrita. |
| fontItalic | Booleano | Indica si la fuente está en cursiva. |
| superior | Int32 | Representa el desplazamiento vertical de la forma desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| izquierda | Int32 | Representa el desplazamiento vertical de la forma desde la esquina superior izquierda en unidades de 1/4000 del área del gráfico. |
| altura | Int32 | Representa la altura de la forma, en unidades de 1/4000 del área del gráfico. |
| ancho | Int32 | Representa el ancho de la forma, en unidades de 1/4000 del área del gráfico. |

### Valor de retorno

Devuelve un objeto Shape que representa el nuevo objeto WordArt.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextEffectInChartWithMsoPresetTextEffectStringStrinDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a la primera hoja de cálculo y agregue datos de muestra
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            
            // Añadir WordArt al gráfico
            Shape wordart = chart.Shapes.AddTextEffectInChart(
                MsoPresetTextEffect.TextEffect2,
                "SAMPLE TEXT", 
                "Arial Black", 
                36, 
                false, 
                false,
                100,  // Left position
                100,  // Top position
                300,  // Width
                200); // Height
                
            // Personalizar la apariencia de WordArt
            wordart.FillFormat.Transparency = 0.7;
            wordart.LineFormat.IsVisible = false;
            
            // Guarda el libro de trabajo
            workbook.Save("WordArtInChart.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


