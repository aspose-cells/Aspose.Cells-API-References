---
title: "CellRichValue.Image"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellRichValue. Obtiene los datos de imagen de la celda"
type: docs
url: /es/net/aspose.cells/cellrichvalue/image/
---
## CellRichValue.Image property

Obtiene los datos de la imagen de la celda.

```csharp
public virtual byte[] Image { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class CellRichValuePropertyImageDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una imagen a la hoja de cálculo
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];

            // Obtener el valor enriquecido de la celda que contiene la imagen
            Cell cell = worksheet.Cells[0, 0];
            cell.PutValue("test data");
            cell.EmbeddedImage = picture.Data;

            // Acceder al valor enriquecido
            CellRichValue richValue = cell.GetRichValue();

            // Mostrar propiedades de la imagen
            Console.WriteLine("Image data length: " + (richValue.Image?.Length ?? 0));
            Console.WriteLine("Alt text: " + richValue.AltText);

            // Establecer nuevo texto alternativo para la imagen
            richValue.AltText = "Sample product image";

            // Guarda el libro de trabajo
            workbook.Save("CellRichValueImageDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


