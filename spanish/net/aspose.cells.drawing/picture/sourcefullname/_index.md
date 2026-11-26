---
title: "Picture.SourceFullName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Picture. Obtiene o establece la ruta y el nombre del archivo fuente para la imagen vinculada"
type: docs
url: /es/net/aspose.cells.drawing/picture/sourcefullname/
---
## Picture.SourceFullName property

Obtiene o establece la ruta y el nombre del archivo fuente para la imagen vinculada.

```csharp
public string SourceFullName { get; set; }
```

### Observaciones

El valor predeterminado es una cadena vacía. Si SourceFullName no es una cadena vacía, la imagen está vinculada. Si SourceFullName no es una cadena vacía, pero Data es nulo, entonces la imagen está vinculada y no se almacena en el archivo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertySourceFullNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una imagen vinculada a la hoja de cálculo
            string imagePath = "example.png";
            Picture picture = worksheet.Shapes.AddLinkedPicture(0, 0, 100, 100, imagePath);

            // Demostrar la propiedad SourceFullName
            Console.WriteLine("Picture SourceFullName: " + picture.SourceFullName);
            Console.WriteLine("Is linked picture: " + picture.IsLink);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


