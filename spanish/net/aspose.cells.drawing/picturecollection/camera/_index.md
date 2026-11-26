---
title: "PictureCollection.Camera"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PictureCollection. Toma una foto del rango"
type: docs
url: /es/net/aspose.cells.drawing/picturecollection/camera/
---
## PictureCollection.Camera method

Toma una foto del rango.

```csharp
public int Camera(int row, int column, string range)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila de esta imagen. |
| columna | Int32 | El índice de columna de esta imagen. |
| rango | String | El área que requiere fotografía |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PictureCollectionMethodCameraWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega algunos datos de muestra para crear un rango
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";
            worksheet.Cells["A2"].Value = "Row 2";
            worksheet.Cells["B2"].Value = "Row 2 Col 2";

            try
            {
                // Obtén la colección Pictures de la hoja de cálculo
                PictureCollection pictures = worksheet.Pictures;

                // Llama al método Camera para crear una imagen de cámara
                // Parámetros: row (fila superior izquierda), column (columna superior izquierda), range (rango de origen)
                int pictureIndex = pictures.Camera(5, 1, "A1:B2");

                Console.WriteLine($"Camera picture added successfully at index: {pictureIndex}");

                // Guarda el libro de trabajo
                workbook.Save("CameraDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Camera method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


