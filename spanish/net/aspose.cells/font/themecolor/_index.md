---
title: "Font.ThemeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Font. Obtiene y establece el color del tema"
type: docs
url: /es/net/aspose.cells/font/themecolor/
---
## Font.ThemeColor property

Obtiene y establece el color del tema.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Observaciones

Si el color de la fuente no es un color de tema, se devolverá NULL.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la celda A1 y establecer el texto
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Theme Color Demo");

            // Obtener el estilo y la fuente
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Crear y establecer el color del tema
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

            // Aplique el estilo a la celda
            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("ThemeColorDemo.xlsx");

            // Verificar el color del tema
            Font savedFont = worksheet.Cells["A1"].GetStyle().Font;
            Console.WriteLine("ThemeColor Type: " + savedFont.ThemeColor.ColorType);
            Console.WriteLine("ThemeColor Tint: " + savedFont.ThemeColor.Tint);
        }
    }
}
```

### Ver también

* class [ThemeColor](../../themecolor/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


