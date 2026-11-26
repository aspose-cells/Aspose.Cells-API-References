---
title: "MsoLineFormatHelper.ForeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoLineFormatHelper. Obtiene y establece el color de primer plano de la línea del borde"
type: docs
url: /es/net/aspose.cells.drawing/msolineformathelper/forecolor/
---
## MsoLineFormatHelper.ForeColor property

Obtiene y establece el color de primer plano de la línea del borde.

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

    public class MsoLineFormatHelperPropertyForeColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una hoja de cálculo de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para que el ejemplo tenga sentido
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crea una forma para demostrar el formato de línea
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Obtener el formato de línea
                MsoLineFormat lineFormat = shape.LineFormat;

                // Mostrar el valor actual de ForeColor
                Console.WriteLine("Current ForeColor: " + lineFormat.ForeColor);

                // Establecer un nuevo ForeColor (ya que es de lectura/escritura)
                lineFormat.ForeColor = Color.Red;
                Console.WriteLine("Updated ForeColor: " + lineFormat.ForeColor);

                // Mostrar cómo la propiedad afecta el comportamiento
                Console.WriteLine("Line fore color has been updated to: " + lineFormat.ForeColor);

                // Guardar el resultado
                workbook.Save("ForeColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line fore color.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


