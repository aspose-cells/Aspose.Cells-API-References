---
title: "LegendEntry.IsDeleted"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LegendEntry. Obtiene y establece si la entrada de leyenda está eliminada"
type: docs
url: /es/net/aspose.cells.charts/legendentry/isdeleted/
---
## LegendEntry.IsDeleted property

Obtiene y establece si la entrada de leyenda está eliminada.

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
    public class LegendEntryPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Obtener la primera entrada de leyenda
            LegendEntry legendEntry = chart.Legend.LegendEntries[0];

            // Demostrar la propiedad IsDeleted
            Console.WriteLine("Legend entry initially deleted? " + legendEntry.IsDeleted);
            
            // Eliminar la entrada de leyenda
            legendEntry.IsDeleted = true;
            Console.WriteLine("Legend entry after deletion? " + legendEntry.IsDeleted);

            // Restaurar la entrada de leyenda
            legendEntry.IsDeleted = false;
            Console.WriteLine("Legend entry after restoration? " + legendEntry.IsDeleted);

            // Guarda el libro de trabajo
            workbook.Save("LegendEntryIsDeletedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


