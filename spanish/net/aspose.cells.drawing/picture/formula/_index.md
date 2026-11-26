---
title: "Picture.Formula"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Picture. Obtiene y establece los datos de la fórmula"
type: docs
url: /es/net/aspose.cells.drawing/picture/formula/
---
## Picture.Formula property

Obtiene y establece los datos de la fórmula.

```csharp
public string Formula { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyFormulaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            // Establece la fórmula para la imagen
            picture.Formula = "A1:A3";
            Console.WriteLine("Picture Formula: " + picture.Formula);

            // Cambia la fórmula
            picture.Formula = "B1:B3";
            Console.WriteLine("Updated Picture Formula: " + picture.Formula);

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


