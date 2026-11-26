---
title: "Axis.HasMultiLevelLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del eje. Indica si las etiquetas se mostrarán como multinivel"
type: docs
url: /es/net/aspose.cells.charts/axis/hasmultilevellabels/
---
## Axis.HasMultiLevelLabels property

Indica si las etiquetas se mostrarán como multinivel.

```csharp
public bool HasMultiLevelLabels { get; set; }
```

### Observaciones

Solo válido para el eje de categorías.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyHasMultiLevelLabelsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo con categorías multinivel
            worksheet.Cells["A1"].PutValue("Main Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Sub Category");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Carrot");
            worksheet.Cells["C1"].PutValue("Value");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(8);
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer el rango de datos del gráfico incluyendo categorías multinivel
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "A1:B3";
            
            // Verificar y mostrar la propiedad HasMultiLevelLabels
            Console.WriteLine("HasMultiLevelLabels: " + chart.CategoryAxis.HasMultiLevelLabels);
            
            // Guarda el libro de trabajo
            workbook.Save("AxisPropertyHasMultiLevelLabelsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


