---
title: "Style.ForegroundThemeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene y establece el color de tema de primer plano"
type: docs
url: /es/net/aspose.cells/style/foregroundthemecolor/
---
## Style.ForegroundThemeColor property

Obtiene y establece el color del tema de primer plano.

```csharp
public ThemeColor ForegroundThemeColor { get; set; }
```

### Observaciones

Si el color de primer plano no es un color de tema, se devolverá NULL.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundThemeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            cells["A1"].PutValue("Foreground Theme Color Demo");
            Style style = cells["A1"].GetStyle();

            style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Accent1, -0.25);
            style.Pattern = BackgroundType.Solid;

            cells["A1"].SetStyle(style);
            workbook.Save("ForegroundThemeColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


