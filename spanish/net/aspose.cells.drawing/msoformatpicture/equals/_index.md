---
title: "MsoFormatPicture.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método MsoFormatPicture."
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/equals/
---
## MsoFormatPicture.Equals method

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

    public class MsoFormatPictureMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar dos imágenes a la hoja de cálculo
            int pictureIndex1 = worksheet.Pictures.Add(0, 0, "example.jpg");
            int pictureIndex2 = worksheet.Pictures.Add(5, 0, "example.jpg");
            
            Picture picture1 = worksheet.Pictures[pictureIndex1];
            Picture picture2 = worksheet.Pictures[pictureIndex2];

            // Obtener los objetos MsoFormatPicture
            MsoFormatPicture format1 = picture1.FormatPicture;
            MsoFormatPicture format2 = picture2.FormatPicture;

            // Establece diferentes propiedades para demostrar la comparación de igualdad
            format1.Brightness = 0.5;
            format1.Contrast = 0.3;
            format2.Brightness = 0.5;
            format2.Contrast = 0.3;

            try
            {
                // Comparar los dos objetos MsoFormatPicture
                bool areEqual = format1.Equals((object)format2);
                Console.WriteLine($"Format objects are equal: {areEqual}");

                // Modificar un formato y comparar de nuevo
                format2.Brightness = 0.7;
                areEqual = format1.Equals((object)format2);
                Console.WriteLine($"After modification, format objects are equal: {areEqual}");

                // Comparar con null
                bool isNullEqual = format1.Equals((object)null);
                Console.WriteLine($"Comparison with null: {isNullEqual}");

                // Comparar con un tipo diferente
                bool isDifferentTypeEqual = format1.Equals((object)"string");
                Console.WriteLine($"Comparison with different type: {isDifferentTypeEqual}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("MsoFormatPictureMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


