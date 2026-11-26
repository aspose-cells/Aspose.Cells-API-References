---
title: "Clase ChartPointCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.ChartPointCollection. Representa una colección que contiene todos los puntos en una serie"
type: docs
url: /es/net/aspose.cells.charts/chartpointcollection/
---
## ChartPointCollection class

Representa una colección que contiene todos los puntos en una serie.

```csharp
public class ChartPointCollection : IEnumerable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Count](../../aspose.cells.charts/chartpointcollection/count/) { get; } | Obtiene el recuento del punto del gráfico. |
| [Item](../../aspose.cells.charts/chartpointcollection/item/) { get; } | Obtiene el elemento [`ChartPoint`](../chartpoint/) en el índice especificado de la serie. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Clear](../../aspose.cells.charts/chartpointcollection/clear/)() | Elimina todas las configuraciones de los puntos del gráfico. |
| [GetEnumerator](../../aspose.cells.charts/chartpointcollection/getenumerator/)() | Devuelve un enumerador para todo el `ChartPointCollection`. |
| [RemoveAt](../../aspose.cells.charts/chartpointcollection/removeat/)(int) | Elimina el punto en el índice de la serie. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointCollectionDemo
    {
        public static void ChartPointCollectionExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Obteniendo la referencia de la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar valores de muestra a celdas
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10);

            // Accediendo a la instancia del gráfico recién agregado
            Chart chart = worksheet.Charts[chartIndex];

            // Añadiendo NSeries (fuente de datos del gráfico) al gráfico desde la celda "A1" hasta "B3"
            chart.NSeries.Add("A1:B3", true);

            // Mostrar etiquetas de datos 
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Accediendo al ChartPointCollection
            ChartPointCollection points = chart.NSeries[0].Points;

            // Iterando a través de los puntos en la colección
            for (int i = 0; i < points.Count; i++)
            {
                // Obtener punto de datos
                ChartPoint point = points[i];
                
                // Establecer explosión de pastel
                point.Explosion = 15;
                
                // Establecer color del borde
                point.Border.Color = System.Drawing.Color.Red;
            }

            // Guardando el archivo Excel
            workbook.Save("ChartPointCollectionExample.xlsx");
            workbook.Save("ChartPointCollectionExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


