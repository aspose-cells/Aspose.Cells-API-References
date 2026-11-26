---
title: "FillFormat.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Obtiene y establece el tipo de relleno"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/type/
---
## FillFormat.Type property

Obtiene y establece el tipo de relleno.

```csharp
[Obsolete("Use FillFormat.FillType  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FillType Type { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad FillFormat.FillType. Esta propiedad será eliminada 12 meses después desde julio de 2016. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);
            FillFormat fill = shape.Fill;

            // Mostrar el valor actual de Type
            Console.WriteLine("Current Type value: " + fill.Type);

            // Cambiar Type a Gradient (propiedad obsoleta usada para demostración)
            fill.Type = FillType.Gradient;

            // Aplicar efecto de degradado de dos colores
            fill.SetTwoColorGradient(Color.Blue, Color.Green, GradientStyleType.Horizontal, 1);

            // Guardar el libro de trabajo modificado
            workbook.Save("FillFormatTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


