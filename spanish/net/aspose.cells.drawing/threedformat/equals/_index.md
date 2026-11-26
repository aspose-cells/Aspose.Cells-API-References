---
title: "ThreeDFormat.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ThreeDFormat."
type: docs
url: /es/net/aspose.cells.drawing/threedformat/equals/
---
## ThreeDFormat.Equals method

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para comparar formatos 3D
            Shape shape1 = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 150, 100, 100, 0, 0);

            // Obtener los formatos 3D de las formas
            ThreeDFormat format1 = shape1.ThreeDFormat;
            ThreeDFormat format2 = shape2.ThreeDFormat;

            // Configurar ajustes 3D idénticos
            format1.BottomBevelWidth = 10;
            format1.BottomBevelHeight = 10;
            format1.BottomBevelType = BevelType.ArtDeco;

            format2.BottomBevelWidth = 10;
            format2.BottomBevelHeight = 10;
            format2.BottomBevelType = BevelType.ArtDeco;

            try
            {
                // Llame al método Equals para comparar los formatos 3D
                bool areEqual = format1.Equals((object)format2);

                // Mostrar el resultado
                Console.WriteLine($"The 3D formats are equal: {areEqual}");

                // Modifique una propiedad para que sean diferentes
                format2.BottomBevelWidth = 15;
                areEqual = format1.Equals((object)format2);
                Console.WriteLine($"After modification, the 3D formats are equal: {areEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("ThreeDFormatEqualsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


