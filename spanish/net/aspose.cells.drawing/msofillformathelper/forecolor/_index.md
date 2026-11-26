---
title: "MsoFillFormatHelper.ForeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "MsoFillFormatHelper property. Obtiene y establece el color de primer plano del relleno"
type: docs
url: /es/net/aspose.cells.drawing/msofillformathelper/forecolor/
---
## MsoFillFormatHelper.ForeColor property

Obtiene y establece el color de primer plano del relleno.

```csharp
public Color ForeColor { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;
    using System.Reflection;

    public class MsoFillFormatHelperPropertyForeColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una etiqueta para que el ejemplo sea significativo
            worksheet.Cells["A1"].Value = "ForeColor Property Demo";

            try
            {
                // Crear una instancia de MsoFillFormatHelper usando reflexión (sin constructor público)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Muestra el valor predeterminado de ForeColor
                Console.WriteLine($"Default ForeColor: {fillHelper.ForeColor}");

                // Establece un nuevo valor de ForeColor
                fillHelper.ForeColor = Color.FromArgb(255, 128, 0, 128); // Purple color
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");

                // Demuestra cómo obtener el valor de ForeColor
                Color currentColor = fillHelper.ForeColor;
                Console.WriteLine($"Current ForeColor (RGB): R={currentColor.R}, G={currentColor.G}, B={currentColor.B}");

                // Guarda el libro de trabajo para demostrar una ejecución exitosa
                workbook.Save("ForeColorDemo.xlsx");

                Console.WriteLine("ForeColor property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColor demo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


