---
title: "LineFormat.JoinType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LineFormat. Especifica el tipo de unión de la línea"
type: docs
url: /es/net/aspose.cells.drawing/lineformat/jointype/
---
## LineFormat.JoinType property

Especifica el tipo de unión de línea.

```csharp
public LineJoinType JoinType { get; set; }
```

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyJoinTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma de línea
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Establecer el tipo de unión de línea a Redondo
            line.Line.JoinType = LineJoinType.Round;

            // Guarda el libro de trabajo
            workbook.Save("LineJoinTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [LineJoinType](../../linejointype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


