---
title: "Chart.ChangeTemplate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método del gráfico. Cambia el tipo de gráfico con una plantilla predefinida"
type: docs
url: /es/net/aspose.cells.charts/chart/changetemplate/
---
## Chart.ChangeTemplate method

Cambiar el tipo de gráfico con una plantilla predefinida.

```csharp
public void ChangeTemplate(byte[] data)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| datos | Byte[] | Los datos del archivo de plantilla de gráfico (.crtx). |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodChangeTemplateWithByteDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", false);

            // Obtener datos de plantilla de otro archivo de gráfico
            byte[] templateData = File.ReadAllBytes("ChartTemplate.crtx");

            try
            {
                // Llamar al método ChangeTemplate con un parámetro de matriz de bytes
                chart.ChangeTemplate(templateData);
                
                Console.WriteLine("Chart template changed successfully using byte array parameter");
                
                // Mostrar el efecto guardando el libro de trabajo
                workbook.Save("ChartWithChangedTemplate.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing chart template: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


