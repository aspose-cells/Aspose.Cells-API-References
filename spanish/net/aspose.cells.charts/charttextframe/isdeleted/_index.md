---
title: "ChartTextFrame.IsDeleted"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartTextFrame. Indica si esta etiqueta de datos está eliminada"
type: docs
url: /es/net/aspose.cells.charts/charttextframe/isdeleted/
---
## ChartTextFrame.IsDeleted property

Indica si esta etiqueta de datos está eliminada.

```csharp
public bool IsDeleted { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder a las etiquetas de datos y demostrar la propiedad IsDeleted
            chart.NSeries[0].DataLabels.ShowValue = true;
            bool isDeletedBefore = chart.NSeries[0].DataLabels.IsDeleted;
            
            // Eliminar las etiquetas de datos estableciendo ShowValue a false
            chart.NSeries[0].DataLabels.ShowValue = false;
            bool isDeletedAfter = chart.NSeries[0].DataLabels.IsDeleted;

            Console.WriteLine($"DataLabels IsDeleted before removal: {isDeletedBefore}");
            Console.WriteLine($"DataLabels IsDeleted after removal: {isDeletedAfter}");
        }
    }
}
```

### Ver también

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


