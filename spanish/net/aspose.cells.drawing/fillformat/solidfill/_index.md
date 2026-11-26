---
title: "FillFormat.SolidFill"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Obtiene el objeto SolidFill"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/solidfill/
---
## FillFormat.SolidFill property

Obtiene el objeto `SolidFill`.

```csharp
public SolidFill SolidFill { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertySolidFillDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 150);
            
            // Establece el color de relleno sólido para la forma
            shape.Fill.SolidFill.Color = System.Drawing.Color.FromArgb(135, 222, 255);
            
            // Obtén y muestra el color de relleno sólido
            System.Drawing.Color fillColor = shape.Fill.SolidFill.Color;
            Console.WriteLine("Solid Fill Color - R:{0}, G:{1}, B:{2}", 
                fillColor.R, fillColor.G, fillColor.B);
            
            // Guarda el libro de trabajo
            workbook.Save("SolidFillDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SolidFill](../../solidfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


