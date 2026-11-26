---
title: "Picture.Move"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Picture. Mueve la imagen a una ubicación especificada"
type: docs
url: /es/net/aspose.cells.drawing/picture/move/
---
## Picture.Move method

Mueve la imagen a una ubicación especificada.

```csharp
public void Move(int topRow, int leftColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodMoveWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            pic.Move(2, 4);
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


