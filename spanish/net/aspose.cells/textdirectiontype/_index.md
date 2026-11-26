---
title: "Enumeración TextDirectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.TextDirectionType. Representa la dirección del flujo de texto para este párrafo"
type: docs
url: /es/net/aspose.cells/textdirectiontype/
---
## TextDirectionType enumeration

Representa la dirección del flujo de texto para este párrafo.

```csharp
public enum TextDirectionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Context | `0` |  |
| LeftToRight | `1` |  |
| RightToLeft | `2` |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTextDirectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Establecer dirección de texto de derecha a izquierda
            Style style = cells["A1"].GetStyle();
            style.TextDirection = TextDirectionType.RightToLeft;
            cells["A1"].SetStyle(style);
            cells["A1"].PutValue("Right to Left Text");

            // Establecer dirección de texto de izquierda a derecha
            style = cells["A2"].GetStyle();
            style.TextDirection = TextDirectionType.LeftToRight;
            cells["A2"].SetStyle(style);
            cells["A2"].PutValue("Left to Right Text");

            // Establecer dirección de texto del contexto
            style = cells["A3"].GetStyle();
            style.TextDirection = TextDirectionType.Context;
            cells["A3"].SetStyle(style);
            cells["A3"].PutValue("Context Text Direction");

            workbook.Save("TextDirectionTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


