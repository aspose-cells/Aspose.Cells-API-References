---
title: "MsoLineFormatHelper.IsVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoLineFormatHelper. Indica si el objeto es visible"
type: docs
url: /es/net/aspose.cells.drawing/msolineformathelper/isvisible/
---
## MsoLineFormatHelper.IsVisible property

Indica si el objeto es visible.

```csharp
public bool IsVisible { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoLineFormatHelperPropertyIsVisibleDemo
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

                // Mostrar el valor actual de IsVisible
                Console.WriteLine("Current IsVisible: " + lineFormat.IsVisible);

                // Establecer un nuevo valor de IsVisible (ya que es de lectura/escritura)
                lineFormat.IsVisible = false;
                Console.WriteLine("Updated IsVisible: " + lineFormat.IsVisible);

                // Mostrar cómo la propiedad afecta el comportamiento
                Console.WriteLine("Line visibility has been updated to: " + lineFormat.IsVisible);

                // Guardar el resultado
                workbook.Save("IsVisibleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line visibility.");
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


