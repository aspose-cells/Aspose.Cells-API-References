---
title: "Picture.IsLink"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Picture. Devuelve verdadero si la imagen está vinculada a un archivo"
type: docs
url: /es/net/aspose.cells.drawing/picture/islink/
---
## Picture.IsLink property

Devuelve true si la imagen está vinculada a un archivo.

```csharp
public bool IsLink { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyIsLinkDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una imagen vinculada
            int linkedPictureIndex = worksheet.Pictures.Add(0, 0, "https://example.com/image.jpg");
            Picture linkedPicture = worksheet.Pictures[linkedPictureIndex];

            // Agregar una imagen incrustada (usando datos de ejemplo)
            byte[] embeddedImageData = new byte[] { 0x01, 0x02, 0x03 }; // Sample image data
            using (MemoryStream stream = new MemoryStream(embeddedImageData))
            {
                int embeddedPictureIndex = worksheet.Pictures.Add(0, 5, stream);
                Picture embeddedPicture = worksheet.Pictures[embeddedPictureIndex];

                // Demostrar la propiedad IsLink
                Console.WriteLine("Linked picture IsLink: " + linkedPicture.IsLink);
                Console.WriteLine("Embedded picture IsLink: " + embeddedPicture.IsLink);

                // Mostrar comportamiento diferente basado en IsLink
                Console.WriteLine("\nLinked picture data is null: " + (linkedPicture.Data == null));
                Console.WriteLine("Embedded picture data length: " + embeddedPicture.Data.Length);
            }
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


