---
title: "TextOptions.FarEastName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextOptions. Obtiene y establece el nombre FarEast"
type: docs
url: /es/net/aspose.cells.drawing.texts/textoptions/fareastname/
---
## TextOptions.FarEastName property

Obtiene y establece el nombre FarEast.

```csharp
public string FarEastName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyFarEastNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma y establecer la fuente FarEastName
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            shape.Text = "Sample Text";
            shape.TextOptions.FarEastName = "宋体";

            // Guarde y recargue para verificar
            string outputPath = "output_FarEastName.xlsx";
            workbook.Save(outputPath);

            // Recargar para verificar
            Workbook verifyWorkbook = new Workbook(outputPath);
            Aspose.Cells.Drawing.Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("FarEastName: " + verifyShape.TextOptions.FarEastName);
        }
    }
}
```

### Ver también

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


