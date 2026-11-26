---
title: "ThemeColor.ColorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThemeColor. Obtiene y establece el tipo de tema"
type: docs
url: /es/net/aspose.cells/themecolor/colortype/
---
## ThemeColor.ColorType property

Obtiene y establece el tipo de tema.

```csharp
public ThemeColorType ColorType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyColorTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear dos colores temáticos con diferentes tipos
            ThemeColor color1 = new ThemeColor(ThemeColorType.Accent1, 0.5);
            ThemeColor color2 = new ThemeColor(ThemeColorType.Accent2, 0.3);
            
            // Demostrar la propiedad ColorType
            Console.WriteLine("Color1 Type: " + color1.ColorType);
            Console.WriteLine("Color2 Type: " + color2.ColorType);
            
            // Aplicar colores temáticos a las celdas
            Style style1 = workbook.CreateStyle();
            style1.ForegroundThemeColor = color1;
            worksheet.Cells["A1"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundThemeColor = color2;
            worksheet.Cells["A2"].SetStyle(style2);
            
            // Guarda el libro de trabajo
            workbook.Save("ThemeColorDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


