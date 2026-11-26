---
title: "MsoLineFormatHelper.Transparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoLineFormatHelper. Devuelve o establece el grado de transparencia del relleno especificado como un valor de 0.0 opaco a 1.0 transparente"
type: docs
url: /es/net/aspose.cells.drawing/msolineformathelper/transparency/
---
## MsoLineFormatHelper.Transparency property

Devuelve o establece el grado de transparencia del relleno especificado como un valor de 0.0 (opaco) a 1.0 (claro).

```csharp
public double Transparency { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyTransparencyDemo
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

                // Mostrar el valor actual de Transparency
                Console.WriteLine("Current Transparency: " + lineFormat.Transparency);

                // Establecer un nuevo valor de Transparency (ya que es de lectura/escritura)
                lineFormat.Transparency = 0.5;
                Console.WriteLine("Updated Transparency: " + lineFormat.Transparency);

                // Mostrar cómo la propiedad afecta el comportamiento
                Console.WriteLine("Line transparency has been updated to: " + lineFormat.Transparency);

                // Guardar el resultado
                workbook.Save("TransparencyDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line transparency.");
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


