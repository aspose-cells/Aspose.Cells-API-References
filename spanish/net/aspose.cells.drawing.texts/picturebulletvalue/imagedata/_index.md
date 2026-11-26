---
title: "PictureBulletValue.ImageData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PictureBulletValue. Obtiene y establece los datos de imagen de la viñeta"
type: docs
url: /es/net/aspose.cells.drawing.texts/picturebulletvalue/imagedata/
---
## PictureBulletValue.ImageData property

Obtiene y establece los datos de imagen de la viñeta.

```csharp
public byte[] ImageData { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.IO;

    public class PictureBulletValuePropertyImageDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Crear una instancia de PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Demostrar la configuración y obtención de ImageData
                byte[] sampleImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample data
                bulletValue.ImageData = sampleImageData;
                
                // Mostrar el valor de la propiedad ImageData
                Console.WriteLine("ImageData length: " + (bulletValue.ImageData?.Length ?? 0) + " bytes");
                
                // Mostrar la propiedad Type (solo lectura)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // Guarda el libro de trabajo
                workbook.Save("PictureBulletValueImageDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


