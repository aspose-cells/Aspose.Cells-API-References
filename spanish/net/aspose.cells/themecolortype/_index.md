---
title: "Enum ThemeColorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.ThemeColorType enum. Enumera los tipos de colores del tema"
type: docs
url: /es/net/aspose.cells/themecolortype/
---
## ThemeColorType enumeration

Enumera los tipos de color de tema.

```csharp
public enum ThemeColorType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Background1 | `0` |  |
| Text1 | `1` |  |
| Background2 | `2` |  |
| Text2 | `3` |  |
| Accent1 | `4` |  |
| Accent2 | `5` |  |
| Accent3 | `6` |  |
| Accent4 | `7` |  |
| Accent5 | `8` |  |
| Accent6 | `9` |  |
| Hyperlink | `10` |  |
| FollowedHyperlink | `11` |  |
| StyleColor | `12` | Inner usado. Un color usado en definiciones de tema que significa usar el color del estilo |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsClassThemeColorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Accede a la celda A1 y obtén su estilo
            Style style = cells["A1"].GetStyle();
            
            // Establece un patrón sólido con color de primer plano rojo
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            Console.WriteLine("Foreground ARGB Color: " + style.ForegroundArgbColor);
            
            // Establece un patrón gray12 con primer plano azul y fondo amarillo
            style.Pattern = BackgroundType.Gray12;
            style.ForegroundColor = Color.Blue;
            style.BackgroundColor = Color.Yellow;
            Console.WriteLine("Foreground ARGB Color: " + style.ForegroundArgbColor);
            Console.WriteLine("Background ARGB Color: " + style.BackgroundArgbColor);
            
            // Establece colores del tema
            ThemeColor foregroundTheme = new ThemeColor(ThemeColorType.Accent6, 0.5);
            ThemeColor backgroundTheme = new ThemeColor(ThemeColorType.Accent2, 0.5);
            style.ForegroundThemeColor = foregroundTheme;
            style.BackgroundThemeColor = backgroundTheme;
            
            Console.WriteLine("Foreground Theme Color Type: " + style.ForegroundThemeColor.ColorType);
            Console.WriteLine("Background Theme Color Type: " + style.BackgroundThemeColor.ColorType);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


