---
title: "Shape.LineFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Shape. Devuelve un objeto MsoLineFormat que contiene propiedades de formato de línea para la forma especificada"
type: docs
url: /es/net/aspose.cells.drawing/shape/lineformat/
---
## Shape.LineFormat property

Devuelve un objeto MsoLineFormat que contiene propiedades de formato de línea para la forma especificada.

```csharp
[Obsolete("Use Shape.Line property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoLineFormat LineFormat { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad Shape.Line. Esta propiedad será eliminada 12 meses después desde julio de 2016. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Añade una forma rectangular a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(3, 0, 2, 0, 70, 130);
            
            // Establecer propiedades de la forma
            rectangle.Placement = PlacementType.FreeFloating;
            rectangle.Fill.FillType = FillType.Solid;
            rectangle.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            
            // Demuestra el uso de LineFormat
            rectangle.LineFormat.Weight = 3; // Set line weight
            rectangle.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            rectangle.Line.SolidFill.Color = System.Drawing.Color.DarkBlue; // Correct way to set line color
            
            // Guarda el libro de trabajo
            workbook.Save("ShapeLineFormatDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoLineFormat](../../msolineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


