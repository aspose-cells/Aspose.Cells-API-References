---
title: "Enum LineCapType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.LineCapType enum. Rappresenta le estremità di una linea"
type: docs
url: /it/net/aspose.cells.drawing/linecaptype/
---
## LineCapType enumeration

Rappresenta le estremità di una linea

```csharp
public enum LineCapType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Square | `0` | Il quadrato sporge per metà della larghezza della linea. |
| Round | `1` | Estremità arrotondate. |
| Flat | `2` | La linea termina al punto finale. |
| None | `3` | Nessun cappuccio |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassLineCapTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);
            
            LineFormat lineFmt = shape.Line;
            lineFmt.CapType = LineCapType.Flat;
            lineFmt.Weight = 2.0;
            lineFmt.DashStyle = MsoLineDashStyle.Solid;
            
            workbook.Save("LineCapTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


