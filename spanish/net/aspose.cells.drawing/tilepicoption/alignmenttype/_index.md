---
title: "TilePicOption.AlignmentType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TilePicOption. Obtiene o establece la alineación para el mosaico"
type: docs
url: /es/net/aspose.cells.drawing/tilepicoption/alignmenttype/
---
## TilePicOption.AlignmentType property

Obtiene o establece la alineación para el mosaico.

```csharp
public RectangleAlignmentType AlignmentType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyAlignmentTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular para demostrar el mosaico
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 300, 300);

            // Configurar el formato de relleno para usar una imagen en mosaico
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // Crear y configurar TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            
            // Mostrar el valor inicial de AlignmentType
            Console.WriteLine("Current AlignmentType: " + tileOptions.AlignmentType);

            // Establecer la alineación a TopRight
            tileOptions.AlignmentType = RectangleAlignmentType.TopRight;
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;

            // Aplicar opciones de mosaico al relleno de la forma
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // Cargar imagen de ejemplo (punto rojo de 1x1 píxel)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // Guardar el libro de trabajo modificado
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo.xlsx");

            // Cambiar la alineación a BottomLeft y guardar otra versión
            tileOptions.AlignmentType = RectangleAlignmentType.BottomLeft;
            workbook.Save("TilePicOptionPropertyAlignmentTypeDemo_BottomLeft.xlsx");
        }
    }
}
```

### Ver también

* enum [RectangleAlignmentType](../../rectanglealignmenttype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


