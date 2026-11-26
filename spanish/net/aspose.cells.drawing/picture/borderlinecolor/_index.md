---
title: "Picture.BorderLineColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Picture. Representa el color de la línea del borde de una imagen"
type: docs
url: /es/net/aspose.cells.drawing/picture/borderlinecolor/
---
## Picture.BorderLineColor property

Representa el color de la línea del borde de una imagen.

```csharp
public Color BorderLineColor { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyBorderLineColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            pic.BorderLineColor = Color.Red;
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


