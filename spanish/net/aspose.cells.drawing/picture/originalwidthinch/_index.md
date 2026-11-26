---
title: "Picture.OriginalWidthInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Picture. Obtiene el ancho original de la imagen en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells.drawing/picture/originalwidthinch/
---
## Picture.OriginalWidthInch property

Obtiene el ancho original de la imagen, en unidades de pulgadas.

```csharp
public double OriginalWidthInch { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una imagen (reemplazar "example.jpg" con la ruta real de su imagen)
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            // Obtener y mostrar el ancho original en pulgadas
            double picWidthInch = pic.OriginalWidthInch;
            Console.WriteLine($"Original picture width: {picWidthInch} inches");
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


