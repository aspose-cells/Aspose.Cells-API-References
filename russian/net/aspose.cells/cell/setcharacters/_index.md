---
title: "Cell.SetCharacters"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Устанавливает формат Rich Text для ячейки"
type: docs
url: /ru/net/aspose.cells/cell/setcharacters/
---
## Cell.SetCharacters method

Устанавливает форматирование RTF ячейки.

```csharp
public void SetCharacters(FontSetting[] characters)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| символы | FontSetting[] | Все объекты Characters. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellMethodSetCharactersWithFontSettingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Установите значение ячейки, чтобы применить форматирование rich text.
            cell.Value = "Hello World!";

            try
            {
                // Создайте настройки шрифта для разных частей текста.
                FontSetting[] fontSettings = new FontSetting[2];

                // Отформатируйте первые 5 символов (Hello) как жирный красный.
                fontSettings[0] = cell.Characters(0, 5);
                fontSettings[0].Font.IsBold = true;
                fontSettings[0].Font.Color = Color.Red;

                // Отформатируйте оставшиеся символы ( World!) как курсивный синий.
                fontSettings[1] = cell.Characters(5, 7);
                fontSettings[1].Font.IsItalic = true;
                fontSettings[1].Font.Color = Color.Blue;

                // Примените настройки отформатированных символов с помощью SetCharacters.
                cell.SetCharacters(fontSettings);

                Console.WriteLine("SetCharacters executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCharacters: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


