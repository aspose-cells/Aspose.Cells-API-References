---
title: "SvgImageOptions.FitToViewPort"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SvgImageOptions. si esta propiedad es verdadera, el svg generado se ajustará al viewport"
type: docs
url: /es/net/aspose.cells.rendering/svgimageoptions/fittoviewport/
---
## SvgImageOptions.FitToViewPort property

Si esta propiedad es verdadera, el SVG generado se ajustará al viewport.

```csharp
public bool FitToViewPort { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;

    public class SvgImageOptionsPropertyFitToViewPortDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rellenar celdas con datos de ejemplo
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 250;

            // Crear un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 18, 6);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            chart.Title.Text = "Sales Report";

            // Crear opciones de renderizado SVG
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Mostrar valor inicial de FitToViewPort
            Console.WriteLine($"Initial FitToViewPort: {svgOptions.FitToViewPort}");

            // Modificar la propiedad y demostrar el efecto
            svgOptions.FitToViewPort = true;
            Console.WriteLine($"Modified FitToViewPort: {svgOptions.FitToViewPort}");

            // Renderizar la hoja de cálculo a SVG con diferentes configuraciones
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortEnabled.svg");

            // Opcional: Crear comparación con FitToViewPort deshabilitado
            svgOptions.FitToViewPort = false;
            renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortDisabled.svg");

            Console.WriteLine("Generated SVG files demonstrate FitToViewPort effect.");
        }
    }
}
```

### Ver también

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


