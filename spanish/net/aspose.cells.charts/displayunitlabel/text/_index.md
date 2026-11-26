---
title: "DisplayUnitLabel.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DisplayUnitLabel. Obtiene o establece el texto de la etiqueta de unidad de visualización"
type: docs
url: /es/net/aspose.cells.charts/displayunitlabel/text/
---
## DisplayUnitLabel.Text property

Obtiene o establece el texto de la etiqueta de unidad de visualización.

```csharp
public override string Text { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DisplayUnitLabelPropertyTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            
            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("A1:A4", true);
            
            // Configurar la etiqueta de unidad de visualización
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Acceder y modificar el texto de la etiqueta de unidad de visualización
            DisplayUnitLabel label = chart.ValueAxis.DisplayUnitLabel;
            Console.WriteLine("Default Display Unit Label: " + label.Text);
            
            // Cambiar el texto
            label.Text = "K Units";
            Console.WriteLine("Modified Display Unit Label: " + label.Text);
            
            // Guarda el libro de trabajo
            workbook.Save("DisplayUnitLabelDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


