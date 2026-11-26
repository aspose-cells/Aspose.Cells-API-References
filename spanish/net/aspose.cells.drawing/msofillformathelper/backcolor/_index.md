---
title: "MsoFillFormatHelper.BackColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "MsoFillFormatHelper property. Obtiene y establece el color de fondo del archivo"
type: docs
url: /es/net/aspose.cells.drawing/msofillformathelper/backcolor/
---
## MsoFillFormatHelper.BackColor property

Obtiene y establece el color de fondo del archivo.

```csharp
public Color BackColor { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyBackColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una etiqueta solo para tener algo de contenido en la hoja
            worksheet.Cells["A1"].Value = "BackColor Property Demo";

            try
            {
                // MsoFillFormatHelper no expone un constructor público, usa reflexión para instanciarlo
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Establece el BackColor a un color conocido (p.ej., LightCoral)
                fillHelper.BackColor = Color.LightCoral;

                // Lee el valor de BackColor y muéstralo
                Console.WriteLine($"BackColor is set to: {fillHelper.BackColor}");

                // Opcionalmente también podrías leer el ForeColor para mostrar que sigue siendo el predeterminado
                Console.WriteLine($"ForeColor (default) : {fillHelper.ForeColor}");

                // Guarda el libro de trabajo – el asistente de relleno no está adjunto a una forma,
                // pero guardar demuestra que el código se ejecutó sin errores.
                workbook.Save("BackColorDemo.xlsx");

                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during BackColor demo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


