---
title: "Clase PictureBulletValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Texts.PictureBulletValue. Representa el valor de la viñeta de imagen"
type: docs
url: /es/net/aspose.cells.drawing.texts/picturebulletvalue/
---
## PictureBulletValue class

Representa el valor de la viñeta de imagen.

```csharp
public class PictureBulletValue : BulletValue
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PictureBulletValue](picturebulletvalue/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ImageData](../../aspose.cells.drawing.texts/picturebulletvalue/imagedata/) { get; set; } | Obtiene y establece los datos de imagen de la viñeta. |
| override [Type](../../aspose.cells.drawing.texts/picturebulletvalue/type/) { get; } | Obtiene el tipo del valor de la viñeta. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;
    using System.IO;

    public class TextsClassPictureBulletValueDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Crea una instancia de la clase PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Carga datos de imagen de muestra (reemplaza con la ruta de imagen real)
                string imagePath = "sample.png";
                if (File.Exists(imagePath))
                {
                    bulletValue.ImageData = File.ReadAllBytes(imagePath);
                    
                    // Mostrar información básica
                    Console.WriteLine($"PictureBulletValue created with Type: {bulletValue.Type}");
                    Console.WriteLine($"Image data length: {bulletValue.ImageData?.Length ?? 0} bytes");
                }
                else
                {
                    Console.WriteLine("Sample image not found, using empty bullet value");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("PictureBulletValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PictureBulletValue: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


