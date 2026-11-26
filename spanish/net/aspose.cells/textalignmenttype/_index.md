---
title: "Enumeración TextAlignmentType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.TextAlignmentType. Enumera los tipos de alineación de texto"
type: docs
url: /es/net/aspose.cells/textalignmenttype/
---
## TextAlignmentType enumeration

Enumera los tipos de alineación de texto.

```csharp
public enum TextAlignmentType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| General | `1792` | Representa la alineación de texto general |
| Bottom | `528` | Representa la alineación de texto inferior |
| Center | `1802` | Representa la alineación de texto centrada |
| CenterAcross | `1286` | Representa la alineación de texto centrada a lo ancho |
| Distributed | `807` | Representa la alineación de texto distribuida |
| Fill | `1284` | Representa la alineación de texto de relleno |
| Justify | `1821` | Representa la alineación de texto justificada |
| Left | `257` | Representa la alineación de texto a la izquierda |
| Right | `259` | Representa la alineación de texto a la derecha. |
| Top | `512` | Representa la alineación de texto superior. |
| JustifiedLow | `832` | Alinea el texto con una longitud de kashida ajustada para texto árabe. |
| ThaiDistributed | `896` | Distribuye el texto tailandés de forma especial, porque cada carácter se trata como una palabra. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TextAlignmentTypeDemo
    {
        public static void TextAlignmentTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(78);

            // Agregar un comentario a una celda
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a comment.";
            comment.TextHorizontalAlignment = TextAlignmentType.Center;
            comment.TextVerticalAlignment = TextAlignmentType.Top;

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Personalizar el título del gráfico
            chart.Title.Text = "Scores Chart";
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            chart.Title.TextVerticalAlignment = TextAlignmentType.Top;

            // Guarda el libro de trabajo
            workbook.Save("TextAlignmentTypeExample.xlsx");

            // Genere la salida de los resultados
            Console.WriteLine("Workbook saved successfully with text alignment settings.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


