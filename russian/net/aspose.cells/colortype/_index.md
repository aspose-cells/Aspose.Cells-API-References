---
title: "Перечисление ColorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ColorType. Представляет все типы цветов"
type: docs
url: /ru/net/aspose.cells/colortype/
---
## ColorType enumeration

Представляет все типы цветов

```csharp
public enum ColorType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Automatic | `0` | Автоматический цвет. |
| AutomaticIndex | `1` | Это автоматический цвет, но отображаемый цвет зависит от настроек ОС. |
| RGB | `2` | RGB‑цвет. |
| IndexedColor | `3` | Индекс цвета в палитре цветов. |
| Theme | `4` | Цвет темы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassColorTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу для демонстрации
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Продемонстрировать использование значений перечисления ColorType
                ColorType automatic = ColorType.Automatic;
                ColorType rgb = ColorType.RGB;
                ColorType theme = ColorType.Theme;

                // Отобразить значения перечисления
                Console.WriteLine($"Automatic color type value: {(int)automatic}");
                Console.WriteLine($"RGB color type value: {(int)rgb}");
                Console.WriteLine($"Theme color type value: {(int)theme}");

                // Создать ячейку и задать её значение
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ColorType Demo");

                // Создать стиль и применить его к ячейке
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Black;
                cell.SetStyle(style);

                // Сохраните книгу
                workbook.Save("ColorTypeDemo.xlsx");

                Console.WriteLine("ColorType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ColorType demonstration: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


