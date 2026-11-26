---
title: "SeriesCollection.ChangeColors"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SeriesCollection. Establecer paleta monocromática para series de gráfico"
type: docs
url: /es/net/aspose.cells.charts/seriescollection/changecolors/
---
## SeriesCollection.ChangeColors method

Establecer paleta monocromática para las series del gráfico.

```csharp
public void ChangeColors(ChartColorPaletteType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | ChartColorPaletteType | El tipo monocromático. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodChangeColorsWithChartColorPaletDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Poblar algunos datos para el gráfico
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["A2"].PutValue("Jan");
            ws.Cells["A3"].PutValue("Feb");
            ws.Cells["A4"].PutValue("Mar");

            ws.Cells["B1"].PutValue("Series1");
            ws.Cells["B2"].PutValue(10);
            ws.Cells["B3"].PutValue(20);
            ws.Cells["B4"].PutValue(30);

            ws.Cells["C1"].PutValue("Series2");
            ws.Cells["C2"].PutValue(15);
            ws.Cells["C3"].PutValue(25);
            ws.Cells["C4"].PutValue(35);

            // Agregar un gráfico de columnas
            int chartIdx = ws.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = ws.Charts[chartIdx];

            // Establecer el rango de datos para la serie
            chart.NSeries.Add("B1:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener la colección de series
            SeriesCollection seriesColl = chart.NSeries;

            try
            {
                // Cambiar la paleta de colores de todas las series en la colección.
                // Utilizar una conversión numérica a un valor de enumeración válido (p.ej., 0) para evitar nombres de miembros de enumeración dependientes.
                seriesColl.ChangeColors((ChartColorPaletteType)0);

                Console.WriteLine("ChangeColors method invoked successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error invoking ChangeColors: {ex.Message}");
            }

            // Guardar el libro de trabajo para verificar el resultado
            workbook.Save("SeriesCollection_ChangeColors_Demo.xlsx");
        }
    }
}
```

### Ver también

* enum [ChartColorPaletteType](../../chartcolorpalettetype/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


