---
title: "Picture.OriginalHeightInch"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Picture. Obtiene la altura original de la imagen en unidades de pulgadas"
type: docs
url: /es/net/aspose.cells.drawing/picture/originalheightinch/
---
## Picture.OriginalHeightInch property

Obtiene la altura original de la imagen, en unidades de pulgadas.

```csharp
public double OriginalHeightInch { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            Console.WriteLine("Original picture height in inches: " + pic.OriginalHeightInch);
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


