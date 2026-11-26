---
title: "Style.SetPatternColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Style. Establece el color de fondo"
type: docs
url: /es/net/aspose.cells/style/setpatterncolor/
---
## Style.SetPatternColor method

Establece el color de fondo.

```csharp
public void SetPatternColor(BackgroundType pattern, Color color1, Color color2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| patrón | BackgroundType | El patrón. |
| color1 | Color | El color de primer plano. |
| color2 | Color | El color de fondo. Solo funciona cuando el patrón no es BackgroundType.None y BackgroundType.Solid. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetPatternColorWithBackgroundTypeColorColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            Style style = cell.GetStyle();
            style.SetPatternColor(BackgroundType.Solid, Color.Red, Color.Blue);
            cell.SetStyle(style);
            
            workbook.Save("SetPatternColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [BackgroundType](../../backgroundtype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


