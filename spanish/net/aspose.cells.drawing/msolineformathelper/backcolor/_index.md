---
title: "MsoLineFormatHelper.BackColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoLineFormatHelper. Obtiene y establece el color de fondo de la línea del borde"
type: docs
url: /es/net/aspose.cells.drawing/msolineformathelper/backcolor/
---
## MsoLineFormatHelper.BackColor property

Obtiene y establece el color de fondo de la línea del borde.

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

    public class MsoLineFormatHelperPropertyBackColorDemo
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

                // Mostrar el valor actual de BackColor
                Console.WriteLine("Current BackColor: " + lineFormat.BackColor);

                // Establecer un nuevo valor de BackColor (ya que es de lectura/escritura)
                lineFormat.BackColor = Color.LightBlue;
                Console.WriteLine("Updated BackColor: " + lineFormat.BackColor);

                // Mostrar cómo la propiedad afecta el comportamiento
                Console.WriteLine("Line back color has been updated to: " + lineFormat.BackColor);

                // Guardar el resultado
                workbook.Save("BackColorDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line back color.");
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


