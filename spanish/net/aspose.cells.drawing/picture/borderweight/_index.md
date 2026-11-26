---
title: "Picture.BorderWeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Picture. Obtiene o establece el grosor de la línea del borde de una imagen en unidades de pt"
type: docs
url: /es/net/aspose.cells.drawing/picture/borderweight/
---
## Picture.BorderWeight property

Obtiene o establece el grosor de la línea del borde de una imagen en unidades de pt.

```csharp
public double BorderWeight { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyBorderWeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Aspose.Cells.Drawing.Picture pic = worksheet.Pictures[imgIndex];
            
            pic.BorderLineColor = Color.Red;
            pic.BorderWeight = 3;
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


