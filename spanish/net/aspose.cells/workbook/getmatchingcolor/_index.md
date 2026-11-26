---
title: "Workbook.GetMatchingColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Workbook. Encuentra el color que mejor coincide en la paleta actual"
type: docs
url: /es/net/aspose.cells/workbook/getmatchingcolor/
---
## Workbook.GetMatchingColor method

Encuentra el Color que mejor coincide en la paleta actual.

```csharp
public Color GetMatchingColor(Color rawColor)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rawColor | Color | Color sin procesar. |

### Valor de retorno

Color que mejor coincide.

### Observaciones

Solo hay 56 colores en la paleta de colores en Excel 97-2003. Si el color no está en la paleta, se establecerá el color similar.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetMatchingColorWithColorDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Comprobar si el color existe en la paleta
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color testColor = Color.FromArgb(255, 123, 123, 123);
            Console.WriteLine("Is custom color in palette: " + workbook.IsColorInPalette(testColor));

            // Obtener color coincidente de la paleta
            Color matchedColor = workbook.GetMatchingColor(testColor);
            Console.WriteLine($"Original color: R={testColor.R}, G={testColor.G}, B={testColor.B}");
            Console.WriteLine($"Matched color: R={matchedColor.R}, G={matchedColor.G}, B={matchedColor.B}");

            // Crear un tema personalizado
            Color[] themeColors = new Color[12];
            for (int i = 0; i < themeColors.Length; i++)
            {
                themeColors[i] = Color.FromArgb(255, 128 + i, 128 + i, 128 + i);
            }
            workbook.CustomTheme("CustomTheme", themeColors);

            // Obtener color del tema
            Color themeColor = workbook.GetThemeColor(ThemeColorType.FollowedHyperlink);
            Console.WriteLine($"Theme color: R={themeColor.R}, G={themeColor.G}, B={themeColor.B}");
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


