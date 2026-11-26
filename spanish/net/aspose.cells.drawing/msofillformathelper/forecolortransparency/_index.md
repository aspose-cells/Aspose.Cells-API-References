---
title: "MsoFillFormatHelper.ForeColorTransparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "MsoFillFormatHelper property. Devuelve o establece el grado del color de primer plano del relleno especificado como un valor de 0.0 opaco a 1.0 transparente"
type: docs
url: /es/net/aspose.cells.drawing/msofillformathelper/forecolortransparency/
---
## MsoFillFormatHelper.ForeColorTransparency property

Devuelve o establece el grado de color de primer plano del relleno especificado como un valor de 0.0 (opaco) a 1.0 (transparente).

```csharp
public double ForeColorTransparency { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyForeColorTransparencyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una etiqueta para que el ejemplo sea significativo
            worksheet.Cells["A1"].Value = "ForeColorTransparency Demo";

            try
            {
                // Crear una instancia de MsoFillFormatHelper usando reflexión (sin constructor público)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Muestra el valor predeterminado de ForeColorTransparency
                Console.WriteLine($"Default ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // Establece un nuevo ForeColor y ForeColorTransparency
                fillHelper.ForeColor = Color.Blue;
                fillHelper.ForeColorTransparency = 0.5; // 50% transparency

                // Muestra los valores actualizados
                Console.WriteLine($"Updated ForeColor: {fillHelper.ForeColor}");
                Console.WriteLine($"Updated ForeColorTransparency: {fillHelper.ForeColorTransparency}");

                // Demuestra la lectura del valor de transparencia
                double transparency = fillHelper.ForeColorTransparency;
                Console.WriteLine($"Current transparency level: {transparency} (0.0=opaque, 1.0=clear)");

                // Guarda el libro de trabajo para demostrar una ejecución exitosa
                workbook.Save("ForeColorTransparencyDemo.xlsx");

                Console.WriteLine("ForeColorTransparency property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ForeColorTransparency demo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


