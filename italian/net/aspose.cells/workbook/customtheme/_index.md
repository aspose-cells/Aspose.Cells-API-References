---
title: "Workbook.CustomTheme"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Personalizza il tema"
type: docs
url: /it/net/aspose.cells/workbook/customtheme/
---
## Workbook.CustomTheme method

Personalizza il tema.

```csharp
public void CustomTheme(string themeName, Color[] colors)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| themeName | String | Il nome del tema |
| colori | Color[] | I colori del tema |

### Osservazioni

La lunghezza dei colori dovrebbe essere 12.

| **Indice dell'array** | **Tipo di tema** |
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
| 10 | Collegamento ipertestuale |
| 11 | Collegamento ipertestuale seguito |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class WorkbookMethodCustomThemeWithStringColorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per dimostrare gli effetti del tema
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Theme Demonstration");
            var style = cell.GetStyle();
            style.Font.IsBold = true;
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Prepara i colori del tema
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
                // Applica tema personalizzato
                workbook.CustomTheme("MyCustomTheme", customColors);

                // Crea una cella formattata per dimostrare l'effetto del tema
                var themedCell = worksheet.Cells["A3"];
                themedCell.PutValue("Themed Text");
                var themedStyle = workbook.CreateStyle();
                themedStyle.Font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.0);
                themedStyle.Font.Size = 12;
                themedCell.SetStyle(themedStyle);

                // Salva la cartella di lavoro
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

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


