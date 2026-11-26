---
title: "FillFormat.SetType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Obtiene el tipo de formato de relleno establecido"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/settype/
---
## FillFormat.SetType property

Obtiene el tipo de formato de relleno establecido.

```csharp
[Obsolete("Use FillFormat.FillType instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FormatSetType SetType { get; set; }
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

    public class FillFormatPropertySetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 200);
            FillFormat fillFormat = shape.Fill;

            Console.WriteLine("Current SetType value: " + fillFormat.SetType);

            fillFormat.SetType = FormatSetType.IsGradientSet;
            fillFormat.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 1);

            Console.WriteLine("New SetType value: " + fillFormat.SetType);

            workbook.Save("FillFormatSetTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FormatSetType](../../formatsettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


