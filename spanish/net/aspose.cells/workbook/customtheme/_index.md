---
title: "Workbook.CustomTheme"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Workbook. Personaliza el tema"
type: docs
url: /es/net/aspose.cells/workbook/customtheme/
---
## Workbook.CustomTheme method

Personaliza el tema.

```csharp
public void CustomTheme(string themeName, Color[] colors)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| themeName | String | El nombre del tema |
| colores | Color[] | Los colores del tema |

### Observaciones

La longitud de los colores debe ser 12.

| **índice de matriz** | **tipo de tema** |
| --- | --- |
| 0 | Backgournd1 |
| 1 | Text1 |
| 2 | Backgournd2 |
| 3 | Text2 |
| 4 | Accent1 |
| 5 | Accent2 |
| 6 | Accent3 |
| 7 | Accent4 |
| 8 | Accent5 |
| 9 | Accent6 |
| 10 | Hipervínculo |
| 11 | Hipervínculo seguido |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class WorkbookMethodCustomThemeWithStringColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra para demostrar los efectos del tema
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Theme Demonstration");
            var style = cell.GetStyle();
            style.Font.IsBold = true;
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Preparar colores del tema
            Color[] customColors = new Color[]
            {
                Color.FromArgb(255, 0, 0),     // Red
                Color.FromArgb(0, 255, 0),     // Green
                Color.FromArgb(0, 0, 255),     // Blue
                Color.FromArgb(255, 255, 0),    // Yellow
                Color.FromArgb(255, 0, 255),    // Magenta
                Color.FromArgb(0, 255, 255),    // Cyan
                Color.FromArgb(128, 0, 128),    // Purple
                Color.FromArgb(128, 128, 0),   // Olive
                Color.FromArgb(0, 128, 128),    // Teal
                Color.FromArgb(128, 0, 0),      // Maroon
                Color.FromArgb(0, 128, 0),     // Green (dark)
                Color.FromArgb(0, 0, 128)       // Navy
            };

            try
            {
                // Aplicar tema personalizado
                workbook.CustomTheme("MyCustomTheme", customColors);

                // Crear una celda con estilo para demostrar el efecto del tema
                var themedCell = worksheet.Cells["A3"];
                themedCell.PutValue("Themed Text");
                var themedStyle = workbook.CreateStyle();
                themedStyle.Font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.0);
                themedStyle.Font.Size = 12;
                themedCell.SetStyle(themedStyle);

                // Guarda el libro de trabajo
                workbook.Save("CustomThemeDemo.xlsx");
            }
            catch (System.Exception ex)
            {
                System.Console.WriteLine($"Error applying custom theme: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


