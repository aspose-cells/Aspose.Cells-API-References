---
title: "ChartCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ChartCollection. Eliminar un gráfico en el índice específico"
type: docs
url: /es/net/aspose.cells.charts/chartcollection/removeat/
---
## ChartCollection.RemoveAt method

Eliminar un gráfico en el índice específico.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice del gráfico. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Mostrar el recuento inicial de gráficos
            Console.WriteLine("Initial chart count: " + sheet.Charts.Count);

            // Eliminar el gráfico en el índice 0
            sheet.Charts.RemoveAt(0);

            // Mostrar el recuento de gráficos después de la eliminación
            Console.WriteLine("Chart count after removal: " + sheet.Charts.Count);
        }
    }
}
```

### Ver también

* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


