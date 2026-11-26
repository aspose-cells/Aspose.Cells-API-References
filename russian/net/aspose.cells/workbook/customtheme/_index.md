---
title: "Workbook.CustomTheme"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Настраивает тему"
type: docs
url: /ru/net/aspose.cells/workbook/customtheme/
---
## Workbook.CustomTheme method

Настраивает тему.

```csharp
public void CustomTheme(string themeName, Color[] colors)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| themeName | String | Имя темы |
| цвета | Color[] | Цвета темы |

### Примечания

Количество цветов должно быть 12.

| **Индекс массива** | **Тип темы** |
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
| 10 | Гиперссылка |
| 11 | Перешедшая гиперссылка |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System.Drawing;

    public class WorkbookMethodCustomThemeWithStringColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать примерные данные для демонстрации эффектов темы
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Theme Demonstration");
            var style = cell.GetStyle();
            style.Font.IsBold = true;
            style.Font.Size = 14;
            cell.SetStyle(style);

            // Подготовить цвета темы
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
                // Применить пользовательскую тему
                workbook.CustomTheme("MyCustomTheme", customColors);

                // Создать стилизованную ячейку для демонстрации эффекта темы
                var themedCell = worksheet.Cells["A3"];
                themedCell.PutValue("Themed Text");
                var themedStyle = workbook.CreateStyle();
                themedStyle.Font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.0);
                themedStyle.Font.Size = 12;
                themedCell.SetStyle(themedStyle);

                // Сохраните книгу
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

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


