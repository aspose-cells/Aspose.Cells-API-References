---
title: "MsoFormatPicture.IsBiLevel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Indica si esta imagen debe mostrarse en blanco y negro de dos colores"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/isbilevel/
---
## MsoFormatPicture.IsBiLevel property

Indica si esta imagen debe mostrarse en blanco y negro de dos colores.

```csharp
public bool IsBiLevel { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyIsBiLevelDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agrega una imagen a la hoja de cálculo
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[index];
            
            // Establecer la imagen a bi-nivel (blanco y negro)
            picture.FormatPicture.IsBiLevel = true;
            
            // Verificar y mostrar el valor de la propiedad IsBiLevel
            Console.WriteLine("Picture is bi-level: " + picture.FormatPicture.IsBiLevel);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


