---
title: "Shape.FillFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Devuelve un objeto MsoFillFormat que contiene propiedades de formato de relleno para la forma especificada"
type: docs
url: /es/net/aspose.cells.drawing/shape/fillformat/
---
## Shape.FillFormat property

Devuelve un objeto MsoFillFormat que contiene propiedades de formato de relleno para la forma especificada.

```csharp
[Obsolete("Use Shape.Fill property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoFillFormat FillFormat { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.Fill. Esta propiedad será eliminada 12 meses después desde julio de 2016. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyFillFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular para demostrar la propiedad FillFormat
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            try
            {
                // Acceder a la propiedad FillFormat (solo lectura)
                MsoFillFormat fillFormat = shape.FillFormat;

                // Mostrar las propiedades actuales de FillFormat
                Console.WriteLine("FillFormat ForeColor: " + fillFormat.ForeColor);
                Console.WriteLine("FillFormat Transparency: " + fillFormat.Transparency);
                Console.WriteLine("FillFormat BackColor: " + fillFormat.BackColor);
                Console.WriteLine("FillFormat IsVisible: " + fillFormat.IsVisible);

                // Modificar las propiedades de FillFormat (ya que no es solo lectura)
                fillFormat.ForeColor = System.Drawing.Color.Red;
                fillFormat.Transparency = 0.5;
                fillFormat.BackColor = System.Drawing.Color.Yellow;
                fillFormat.IsVisible = true;

                // Mostrar las propiedades actualizadas de FillFormat
                Console.WriteLine("Updated FillFormat ForeColor: " + fillFormat.ForeColor);
                Console.WriteLine("Updated FillFormat Transparency: " + fillFormat.Transparency);
                Console.WriteLine("Updated FillFormat BackColor: " + fillFormat.BackColor);
                Console.WriteLine("Updated FillFormat IsVisible: " + fillFormat.IsVisible);

                // Guarda el libro de trabajo
                workbook.Save("FillFormatDemo.xlsx");
                Console.WriteLine("FillFormat has been demonstrated and workbook saved.");
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

* class [MsoFillFormat](../../msofillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


