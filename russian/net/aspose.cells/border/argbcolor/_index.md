---
title: "Border.ArgbColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Border. Получает и задает цвет с 32‑битовым значением ARGB"
type: docs
url: /ru/net/aspose.cells/border/argbcolor/
---
## Border.ArgbColor property

Получает и задаёт цвет в виде 32‑битного значения ARGB.

```csharp
public int ArgbColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyArgbColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Обратиться к ячейке B2 и установить значение
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Border ARGB Color Demo");

            // Получить стиль и границы
            Style style = cell.GetStyle();
            Border border = style.Borders[BorderType.TopBorder];

            // Установить свойства границы, включая цвет ARGB
            border.LineStyle = CellBorderType.Thick;
            unchecked
            {
                border.ArgbColor = (int)0xFFFF0000; // Red color in ARGB format with unchecked cast
            }

            // Применить изменённый стиль к ячейке
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("BorderArgbColorDemo.xlsx");

            // Проверить, что цвет ARGB установлен правильно
            Border savedBorder = workbook.Worksheets[0].Cells["B2"].GetStyle().Borders[BorderType.TopBorder];
            Console.WriteLine("ARGB Color of top border: " + savedBorder.ArgbColor.ToString("X8"));
        }
    }
}
```

### См. также

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


