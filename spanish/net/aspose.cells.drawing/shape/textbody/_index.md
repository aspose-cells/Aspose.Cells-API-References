---
title: "Shape.TextBody"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece la configuración del texto de la forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/textbody/
---
## Shape.TextBody property

Obtiene y establece la configuración del texto de la forma.

```csharp
public FontSettingCollection TextBody { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextBodyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);
            FontSettingCollection fontSettingCollection = shape.TextBody;
            fontSettingCollection.Text = "This is a test.";

            workbook.Save("ShapeTextBodyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FontSettingCollection](../../../aspose.cells.drawing.texts/fontsettingcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


