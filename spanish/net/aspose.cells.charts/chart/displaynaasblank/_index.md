---
title: "Chart.DisplayNaAsBlank"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Indica si se debe mostrar N/A como un valor en blanco"
type: docs
url: /es/net/aspose.cells.charts/chart/displaynaasblank/
---
## Chart.DisplayNaAsBlank property

Indica si se debe mostrar #N/A como un valor en blanco.

```csharp
public bool DisplayNaAsBlank { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyDisplayNaAsBlankDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra con algunos valores NA
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(double.NaN); // NA value
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer la propiedad DisplayNaAsBlank
            chart.DisplayNaAsBlank = true;

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            // Verificar la propiedad
            Console.WriteLine("DisplayNaAsBlank is set to: " + chart.DisplayNaAsBlank);
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


