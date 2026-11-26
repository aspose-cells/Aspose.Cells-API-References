---
title: "Border.ThemeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Border. Obtiene y establece el color temático del borde"
type: docs
url: /es/net/aspose.cells/border/themecolor/
---
## Border.ThemeColor property

Obtiene y establece el color temático del borde.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a una celda y obtener su estilo
            Style style = worksheet.Cells["A1"].GetStyle();

            // Establecer color temático del borde
            style.Borders[BorderType.BottomBorder].ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Aplique el estilo a la celda
            worksheet.Cells["A1"].SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("BorderThemeColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ThemeColor](../../themecolor/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


