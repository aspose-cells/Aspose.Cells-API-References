---
title: "MsoLineFormatHelper.Weight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoLineFormatHelper. Obtiene o establece el grosor de la línea en unidades de pt"
type: docs
url: /es/net/aspose.cells.drawing/msolineformathelper/weight/
---
## MsoLineFormatHelper.Weight property

Devuelve o establece el grosor de la línea, en unidades de pt.

```csharp
public double Weight { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineFormatHelperPropertyWeightDemo
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

                // Mostrar el valor actual de Weight
                Console.WriteLine("Current Line Weight: " + lineFormat.Weight);

                // Establecer un nuevo valor de Weight (ya que es de lectura/escritura)
                lineFormat.Weight = 2.5;
                Console.WriteLine("Updated Line Weight: " + lineFormat.Weight);

                // Mostrar cómo la propiedad afecta el comportamiento
                Console.WriteLine("Line weight has been updated to: " + lineFormat.Weight);

                // Guardar el resultado
                workbook.Save("WeightDemo.xlsx");
                Console.WriteLine("File saved successfully with updated line weight.");
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


