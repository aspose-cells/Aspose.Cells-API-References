---
title: "TilePicOption.MirrorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TilePicOption. Obtiene o establece el tipo de espejo para el mosaico"
type: docs
url: /es/net/aspose.cells.drawing/tilepicoption/mirrortype/
---
## TilePicOption.MirrorType property

Obtiene o establece el tipo de espejo para el mosaico.

```csharp
public MirrorType MirrorType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class TilePicOptionPropertyMirrorTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 500, 500, 500);

            // Carga datos de imagen de muestra (reemplaza con la ruta de imagen real)
            byte[] imageData = File.ReadAllBytes("sample.png");

            // Crear y configurar una instancia de TilePicOption
            TilePicOption tileOptions = new TilePicOption();

            // Mostrar el valor inicial de MirrorType
            Console.WriteLine("Current MirrorType: " + tileOptions.MirrorType);

            // Configura las opciones de mosaico
            tileOptions.ScaleX = 0.5;
            tileOptions.ScaleY = 0.5;
            tileOptions.MirrorType = MirrorType.Both;

            // Aplicar la configuración de mosaico usando las propiedades correctas
            shape.Fill.FillType = FillType.Texture;
            shape.Fill.ImageData = imageData;
            shape.Fill.TextureFill.TilePicOption = tileOptions;

            // Guardar el libro de trabajo modificado
            workbook.Save("TilePicOptionMirrorTypeDemo.xlsx");

            Console.WriteLine("Updated MirrorType: " + tileOptions.MirrorType);
        }
    }
}
```

### Ver también

* enum [MirrorType](../../mirrortype/)
* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


