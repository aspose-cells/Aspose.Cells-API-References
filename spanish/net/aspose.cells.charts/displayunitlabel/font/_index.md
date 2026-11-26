---
title: "DisplayUnitLabel.Font"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DisplayUnitLabel. Obtiene un objeto Font del objeto ChartFrame especificado"
type: docs
url: /es/net/aspose.cells.charts/displayunitlabel/font/
---
## DisplayUnitLabel.Font property

Obtiene un objeto `Font` del objeto ChartFrame especificado.

```csharp
public override Font Font { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DisplayUnitLabelPropertyFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            worksheet.Cells["A5"].PutValue(5000);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A5", true);

            // Establecer unidades de visualización para el eje de valores
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            chart.ValueAxis.DisplayUnitLabel.Text = "Thousands";

            // Obtener la instancia de DisplayUnitLabel
            DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;

            // Mostrar propiedades actuales de la fuente
            Font currentFont = displayUnitLabel.Font;
            Console.WriteLine("Current Font Properties:");
            Console.WriteLine($"Name: {currentFont.Name}");
            Console.WriteLine($"Size: {currentFont.Size}");
            Console.WriteLine($"Color: {currentFont.Color}");
            Console.WriteLine($"Bold: {currentFont.IsBold}");
            Console.WriteLine($"Italic: {currentFont.IsItalic}");

            // Crear un nuevo estilo de fuente y aplicarlo a DisplayUnitLabel
            // Nota: Dado que Font es de solo lectura, modificamos sus propiedades directamente
            currentFont.Name = "Arial";
            currentFont.Size = 12;
            currentFont.Color = System.Drawing.Color.Red;
            currentFont.IsBold = true;
            currentFont.IsItalic = false;
            currentFont.Underline = FontUnderlineType.Single;

            // Guarda el libro de trabajo para ver los cambios
            workbook.Save("DisplayUnitLabelFontDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Font](../../../aspose.cells/font/)
* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


