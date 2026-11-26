---
title: "Picture.DisplayAsIcon"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Picture. Verdadero si el objeto especificado se muestra como un ícono y la imagen no se cambiará automáticamente"
type: docs
url: /es/net/aspose.cells.drawing/picture/displayasicon/
---
## Picture.DisplayAsIcon property

True si el objeto especificado se muestra como un ícono y la imagen no se cambiará automáticamente.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int pictureIndex = worksheet.Pictures.Add(1, 1, "example.ico");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Establecer la propiedad DisplayAsIcon a verdadero
            picture.DisplayAsIcon = true;
            
            // Establecer otras propiedades de la imagen
            picture.Name = "IconDisplay";
            picture.Height = 100;
            picture.Width = 100;

            // Guarda el libro de trabajo
            workbook.Save("DisplayAsIconDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon display picture.");
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


