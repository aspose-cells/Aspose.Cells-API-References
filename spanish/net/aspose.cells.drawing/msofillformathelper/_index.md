---
title: "Clase MsoFillFormatHelper"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.MsoFillFormatHelper class. Representa el formato de relleno para una forma"
type: docs
url: /es/net/aspose.cells.drawing/msofillformathelper/
---
## MsoFillFormatHelper class

Representa el formato de relleno para una forma.

```csharp
public class MsoFillFormatHelper
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msofillformathelper/backcolor/) { get; set; } | Obtiene y establece el color de fondo del archivo. |
| [ForeColor](../../aspose.cells.drawing/msofillformathelper/forecolor/) { get; set; } | Obtiene y establece el color de primer plano del relleno. |
| [ForeColorTransparency](../../aspose.cells.drawing/msofillformathelper/forecolortransparency/) { get; set; } | Devuelve o establece el grado de color de primer plano del relleno especificado como un valor de 0.0 (opaco) a 1.0 (transparente). |
| [ImageData](../../aspose.cells.drawing/msofillformathelper/imagedata/) { get; set; } | Obtiene y establece los datos de relleno de textura y de imagen. |
| [IsVisible](../../aspose.cells.drawing/msofillformathelper/isvisible/) { get; set; } | Indica si hay relleno. |
| [Texture](../../aspose.cells.drawing/msofillformathelper/texture/) { get; } | Obtiene el tipo de relleno de textura. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetOneColorGradient](../../aspose.cells.drawing/msofillformathelper/setonecolorgradient/)(Color, double, GradientStyleType, int) | Establece el relleno especificado a un degradado de un solo color. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;
    using System.Reflection;

    public class DrawingClassMsoFillFormatHelperDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "MsoFillFormatHelper Demo";

            try
            {
                // Crea una instancia de MsoFillFormatHelper usando reflexión
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Establecer propiedades básicas
                fillHelper.ForeColor = Color.FromArgb(255, 100, 150, 200);
                fillHelper.ForeColorTransparency = 0.3;
                fillHelper.BackColor = Color.LightGray;
                fillHelper.IsVisible = true;

                // Mostrar valores de propiedades
                Console.WriteLine($"ForeColor: {fillHelper.ForeColor}");
                Console.WriteLine($"ForeColorTransparency: {fillHelper.ForeColorTransparency}");
                Console.WriteLine($"BackColor: {fillHelper.BackColor}");
                Console.WriteLine($"IsVisible: {fillHelper.IsVisible}");
                Console.WriteLine($"Texture (read-only): {fillHelper.Texture}");

                // Guarda el libro de trabajo
                workbook.Save("MsoFillFormatHelperDemo.xlsx");
                Console.WriteLine("MsoFillFormatHelper demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in MsoFillFormatHelper demo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


