---
title: "Chart.Calculate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Chart método. Calcula las posiciones personalizadas del área de trazado y los ejes si sus posiciones se asignan automáticamente"
type: docs
url: /es/net/aspose.cells.charts/chart/calculate/
---
## Calculate() {#calculate}

Calcula las posiciones personalizadas del área de trazado y los ejes si sus posiciones se asignan automáticamente.

```csharp
public void Calculate()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodCalculateDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular el gráfico antes de guardar
            chart.Calculate();

            // Guardar el libro de trabajo con el gráfico
            workbook.Save("ChartCalculateDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Calculate(ChartCalculateOptions) {#calculate_1}

Calcula la posición personalizada del área de trazado y los ejes si su posición se asigna automáticamente, con Opciones de cálculo del gráfico.

```csharp
public void Calculate(ChartCalculateOptions calculateOptions)
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodCalculateWithChartCalculateOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(150);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Habilitar etiquetas de datos
            chart.NSeries[0].DataLabels.ShowValue = true;

            // Crear opciones de cálculo y configurarlas para actualizar todos los puntos
            ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
            calculateOptions.UpdateAllPoints = true;

            // Calcular gráfico con opciones
            chart.Calculate(calculateOptions);

            // Generar los textos de etiquetas de datos
            ChartPointCollection points = chart.NSeries[0].Points;
            Console.WriteLine("DataLabel Text for Point 0: " + points[0].DataLabels.Text);
            Console.WriteLine("DataLabel Text for Point 1: " + points[1].DataLabels.Text);
            Console.WriteLine("DataLabel Text for Point 2: " + points[2].DataLabels.Text);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ChartCalculateOptions](../../chartcalculateoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


