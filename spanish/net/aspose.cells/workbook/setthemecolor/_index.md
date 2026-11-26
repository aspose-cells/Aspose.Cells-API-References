---
title: "Workbook.SetThemeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Workbook method. Establece el color del tema"
type: docs
url: /es/net/aspose.cells/workbook/setthemecolor/
---
## Workbook.SetThemeColor method

Establece el color del tema

```csharp
public void SetThemeColor(ThemeColorType type, Color color)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | ThemeColorType | El tipo de color del tema. |
| color | Color | el color del tema |

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetThemeColorWithThemeColorTypeColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establecer el color del tema para Text1 a Verde
            workbook.SetThemeColor(ThemeColorType.Text1, Color.Green);
            
            // Aplicar el color del tema al estilo predeterminado
            Style style = workbook.DefaultStyle;
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text1, 0);
            workbook.DefaultStyle = style;
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Workbook with theme color saved successfully.");
        }
    }
}
```

### Ver también

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


