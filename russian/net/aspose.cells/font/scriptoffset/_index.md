---
title: "Font.ScriptOffset"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Font. Получает и задает смещение скрипта в процентах"
type: docs
url: /ru/net/aspose.cells/font/scriptoffset/
---
## Font.ScriptOffset property

Получает и задает смещение скрипта в процентах

```csharp
public double ScriptOffset { get; set; }
```

### Примечания

Только для фигур и диаграмм.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyScriptOffsetDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к ячейке A1 и установить её значение
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("ScriptOffset Demo");

            // Получить стиль и шрифт ячейки
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Установить ScriptOffset, чтобы продемонстрировать эффект нижнего/верхнего индекса
            font.ScriptOffset = 10; // Positive for superscript, negative for subscript
            font.IsSuperscript = true; // Enable superscript

            // Применить изменённый стиль к ячейке
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("FontScriptOffsetDemo.xlsx");

            // Проверить значение ScriptOffset
            Console.WriteLine("ScriptOffset value: " + font.ScriptOffset);
        }
    }
}
```

### См. также

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


