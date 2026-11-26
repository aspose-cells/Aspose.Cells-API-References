---
title: "MsoFormatPicture.Transparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Devuelve o establece el grado de transparencia del área como un valor de 0.0 opaco a 1.0 transparente"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/transparency/
---
## MsoFormatPicture.Transparency property

Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (claro).

```csharp
public double Transparency { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar dos imágenes a la hoja de cálculo
            int index1 = worksheet.Pictures.Add(0, 0, "image1.png");
            int index2 = worksheet.Pictures.Add(2, 0, "image2.png");

            // Establecer la transparencia para las imágenes
            worksheet.Pictures[index1].FormatPicture.Transparency = 0.5;
            worksheet.Pictures[index2].FormatPicture.Transparency = 0.69;

            // Guardar y volver a cargar el libro de trabajo para verificar la configuración de transparencia
            string outputPath = "output.xlsx";
            workbook.Save(outputPath);
            
            Workbook loadedWorkbook = new Workbook(outputPath);
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];

            // Mostrar los valores de transparencia en la consola
            Console.WriteLine("Picture 1 Transparency: " + loadedWorksheet.Pictures[0].FormatPicture.Transparency);
            Console.WriteLine("Picture 2 Transparency: " + loadedWorksheet.Pictures[1].FormatPicture.Transparency);
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


