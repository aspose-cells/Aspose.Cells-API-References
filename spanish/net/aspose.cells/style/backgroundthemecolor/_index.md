---
title: "Style.BackgroundThemeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Style. Obtiene y establece el color de tema de fondo"
type: docs
url: /es/net/aspose.cells/style/backgroundthemecolor/
---
## Style.BackgroundThemeColor property

Obtiene y establece el color del tema de fondo.

```csharp
public ThemeColor BackgroundThemeColor { get; set; }
```

### Observaciones

Si el color de fondo no es un color de tema, se devolverá NULL.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundThemeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crear un estilo y establecer el color de tema de fondo
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent2, 0.5);
            style.BackgroundThemeColor = themeColor;

            // Aplicar el estilo a una celda
            cells["A1"].SetStyle(style);

            // Verificar el color de tema de fondo
            ThemeColor retrievedColor = cells["A1"].GetStyle().BackgroundThemeColor;
            Console.WriteLine("Background Theme Color Type: " + retrievedColor.ColorType);
            Console.WriteLine("Background Theme Color Tint: " + retrievedColor.Tint);
        }
    }
}
```

### Ver también

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


