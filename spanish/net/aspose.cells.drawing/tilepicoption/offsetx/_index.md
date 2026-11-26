---
title: "TilePicOption.OffsetX"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TilePicOption. Obtiene o establece el desplazamiento X para la imagen de mosaico"
type: docs
url: /es/net/aspose.cells.drawing/tilepicoption/offsetx/
---
## TilePicOption.OffsetX property

Obtiene o establece el desplazamiento X para la imagen de mosaico.

```csharp
public double OffsetX { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TilePicOptionPropertyOffsetXDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular para demostrar el mosaico
            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);

            // Configurar el formato de relleno para usar una imagen en mosaico
            FillFormat fillFormat = rectangle.Fill;
            fillFormat.FillType = FillType.Texture;

            // Crear y configurar TilePicOption
            TilePicOption tileOptions = new TilePicOption();
            
            // Leer el valor inicial de OffsetX
            Console.WriteLine("Current OffsetX value: " + tileOptions.OffsetX);

            // Establecer un nuevo desplazamiento X para el patrón de mosaico
            tileOptions.OffsetX = 15.5;

            // Aplicar opciones de mosaico al relleno de la forma
            fillFormat.TextureFill.TilePicOption = tileOptions;

            // Cargar una imagen mínima de 1x1 píxel (punto rojo)
            byte[] imageData = Convert.FromBase64String(
                "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
            fillFormat.ImageData = imageData;

            // Guardar el libro de trabajo modificado
            workbook.Save("TilePicOptionPropertyOffsetXDemo.xlsx");
        }
    }
}
```

### Ver también

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


