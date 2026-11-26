---
title: "Cell.EmbeddedImage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene y establece la imagen incrustada en la celda"
type: docs
url: /es/net/aspose.cells/cell/embeddedimage/
---
## Cell.EmbeddedImage property

Obtiene y establece la imagen incrustada en la celda.

```csharp
public byte[] EmbeddedImage { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellPropertyEmbeddedImageDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Elija una celda para almacenar la imagen incrustada
                Cell cell = worksheet.Cells["B2"];

                // Un PNG transparente de 1x1 píxel (codificado en Base64)
                const string pngBase64 =
                    "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mP8/x8AAwMCAO2b4ZcAAAAASUVORK5CYII=";

                // Convertir la cadena Base64 a una matriz de bytes
                byte[] imageBytes = Convert.FromBase64String(pngBase64);

                // Establecer la imagen incrustada en la celda
                cell.EmbeddedImage = imageBytes;

                // Recuperar la imagen incrustada de la celda
                byte[] retrievedBytes = cell.EmbeddedImage;

                // Escribir la imagen recuperada en un archivo para verificar que se almacenó correctamente
                string outputImagePath = "EmbeddedImage_Output.png";
                File.WriteAllBytes(outputImagePath, retrievedBytes);

                Console.WriteLine($"Embedded image byte length: {retrievedBytes.Length}");
                Console.WriteLine($"Embedded image saved to: {Path.GetFullPath(outputImagePath)}");

                // Guardar el libro de trabajo (la imagen incrustada se almacena dentro del .xlsx)
                string workbookPath = "EmbeddedImageDemo.xlsx";
                workbook.Save(workbookPath);
                Console.WriteLine($"Workbook saved to: {Path.GetFullPath(workbookPath)}");
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

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


