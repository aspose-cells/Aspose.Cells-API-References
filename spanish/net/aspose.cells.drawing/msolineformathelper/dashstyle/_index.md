---
title: "MsoLineFormatHelper.DashStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoLineFormatHelper. Obtiene o establece el estilo de guión para la línea especificada"
type: docs
url: /es/net/aspose.cells.drawing/msolineformathelper/dashstyle/
---
## MsoLineFormatHelper.DashStyle property

Obtiene o establece el estilo de guión para la línea especificada.

```csharp
public MsoLineDashStyle DashStyle { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyDashStyleDemo
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

                // Mostrar el valor actual de DashStyle
                Console.WriteLine("Current DashStyle: " + lineFormat.DashStyle);

                // Establecer un nuevo valor de DashStyle (ya que es de lectura/escritura)
                lineFormat.DashStyle = MsoLineDashStyle.DashDot;
                Console.WriteLine("Updated DashStyle: " + lineFormat.DashStyle);

                // Mostrar cómo la propiedad afecta el comportamiento
                Console.WriteLine("Line dash style has been updated to: " + lineFormat.DashStyle);

                // Guardar el resultado
                workbook.Save("DashStyleDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line dash style.");
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

* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


