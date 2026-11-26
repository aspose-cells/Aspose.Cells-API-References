---
title: "Range.ApplyStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Aplica formatos a todo un rango"
type: docs
url: /es/net/aspose.cells/range/applystyle/
---
## Range.ApplyStyle method

Aplica formatos a todo un rango.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | El objeto de estilo que se aplicará. |
| bandera | StyleFlag | Banderas que indican las propiedades de formato aplicadas. |

### Observaciones

Cada celda en este rango contendrá un objeto [`Style`](../../style/). Por lo tanto, este es un método que consume mucha memoria. Por favor, úselo con cuidado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;

            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue("Sample text for style demonstration");

            Aspose.Cells.Range range = cells.CreateRange(0, 0, 1, 3);

            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HorizontalAlignment = true;
            styleFlag.VerticalAlignment = true;
            styleFlag.WrapText = true;

            range.ApplyStyle(style, styleFlag);

            workbook.Save("ApplyStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


