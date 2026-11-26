---
title: "CellsHelper.GetTextWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Obtiene el ancho del texto en unidades de puntos"
type: docs
url: /es/net/aspose.cells/cellshelper/gettextwidth/
---
## CellsHelper.GetTextWidth method

Obtiene el ancho del texto en unidades de puntos.

```csharp
public static double GetTextWidth(string text, Font font, double scaling)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | String | El texto. |
| fuente | Fuente | La fuente del texto. |
| escalado | Double | El escalado del texto. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetTextWidthWithStringFontDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Font font = workbook.DefaultStyle.Font;
            double textWidth = CellsHelper.GetTextWidth("Sample Text", font, 1.0);
            Console.WriteLine("Text width: " + textWidth);
        }
    }
}
```

### Ver también

* class [Font](../../font/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


