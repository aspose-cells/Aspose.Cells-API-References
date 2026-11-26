---
title: "MsoLineFormatHelper.Style"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoLineFormatHelper. Devuelve un objeto Style que representa el estilo del rango especificado"
type: docs
url: /es/net/aspose.cells.drawing/msolineformathelper/style/
---
## MsoLineFormatHelper.Style property

Devuelve un objeto Style que representa el estilo del rango especificado.

```csharp
public MsoLineStyle Style { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyStyleDemo
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

                // Obtener el formato de línea directamente (MsoLineFormatHelper parece ser una clase auxiliar)
                // Dado que no podemos instanciar MsoLineFormatHelper directamente, trabajaremos con la propiedad LineFormat
                MsoLineFormat lineFormat = shape.LineFormat;

                // Mostrar el valor actual de Style
                Console.WriteLine("Current Line Style: " + lineFormat.Style);

                // Establecer un nuevo estilo (ya que Style es de lectura/escritura)
                lineFormat.Style = MsoLineStyle.ThickBetweenThin;
                Console.WriteLine("Updated Line Style: " + lineFormat.Style);

                // Mostrar cómo la propiedad afecta el comportamiento
                Console.WriteLine("Line style has been updated to: " + lineFormat.Style);

                // Guardar el resultado
                workbook.Save("LineStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line style.");
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

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


