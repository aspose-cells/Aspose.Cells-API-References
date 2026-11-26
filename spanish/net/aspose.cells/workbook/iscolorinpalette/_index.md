---
title: "Workbook.IsColorInPalette"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Verifica si un color está en la paleta para la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/workbook/iscolorinpalette/
---
## Workbook.IsColorInPalette method

Comprueba si un color está en la paleta de la hoja de cálculo.

```csharp
public bool IsColorInPalette(Color color)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| color | Color | Estructura Color. |

### Valor de retorno

Devuelve true si este color está en la paleta. De lo contrario, devuelve false

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodIsColorInPaletteWithColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Comprobar si el color estándar existe en la paleta
            bool isRedInPalette = workbook.IsColorInPalette(Color.Red);
            Console.WriteLine("Is Red in palette: " + isRedInPalette);
            
            // Comprobar si el color personalizado existe en la paleta
            Color customColor = Color.FromArgb(255, 123, 123, 123);
            bool isCustomInPalette = workbook.IsColorInPalette(customColor);
            Console.WriteLine("Is custom color in palette: " + isCustomInPalette);
            
            // Obtener color coincidente de la paleta
            Color matchedColor = workbook.GetMatchingColor(customColor);
            Console.WriteLine("Matched color R value: " + matchedColor.R);
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


