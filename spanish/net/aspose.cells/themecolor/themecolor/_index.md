---
title: "ThemeColor.ThemeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de ThemeColor."
type: docs
url: /es/net/aspose.cells/themecolor/themecolor/
---
## ThemeColor constructor

```csharp
public ThemeColor(ThemeColorType type, double tint)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | ThemeColorType | El tipo de tema. |
| tinte | Double | El valor del tinte. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorMethodCtorWithThemeColorTypeDoubleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Llamar al método #ctor con los parámetros ThemeColorType y Double
                ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // Aplicar el color temático al estilo de una celda
                Style style = workbook.CreateStyle();
                style.ForegroundThemeColor = themeColor;
                style.Pattern = BackgroundType.Solid;
                
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ThemeColor with Accent1 and 0.5 tint");
                cell.SetStyle(style);

                Console.WriteLine("ThemeColor constructor executed successfully with parameters (ThemeColorType.Accent1, 0.5)");
                Console.WriteLine($"ColorType: {themeColor.ColorType}, Tint: {themeColor.Tint}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ThemeColor constructor: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("ThemeColorCtorDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


