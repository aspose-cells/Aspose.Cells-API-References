---
title: "DisplayUnitLabel.AutoScaleFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DisplayUnitLabel. Verdadero si el texto en el objeto cambia el tamaño de fuente cuando el tamaño del objeto cambia. El valor predeterminado es Verdadero"
type: docs
url: /es/net/aspose.cells.charts/displayunitlabel/autoscalefont/
---
## DisplayUnitLabel.AutoScaleFont property

True si el texto en el objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor predeterminado es True.

```csharp
public override bool AutoScaleFont { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DisplayUnitLabelPropertyAutoScaleFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Configurar la etiqueta de unidad de visualización
            chart.ValueAxis.DisplayUnit = Aspose.Cells.Charts.DisplayUnitType.Hundreds;
            Aspose.Cells.Charts.DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;
            
            // Demostrar la propiedad AutoScaleFont
            displayUnitLabel.AutoScaleFont = true;
            displayUnitLabel.Text = "100";

            workbook.Save("DisplayUnitLabelAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


