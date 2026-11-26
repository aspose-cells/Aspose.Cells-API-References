---
title: "FontSetting.TextOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FontSetting. Возвращает параметры текста"
type: docs
url: /ru/net/aspose.cells/fontsetting/textoptions/
---
## FontSetting.TextOptions property

Возвращает параметры текста.

```csharp
public TextOptions TextOptions { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyTextOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать пример текста с различными секциями форматирования
            string part1 = "This is normal text. ";
            string part2 = "This is bold and italic text. ";
            string part3 = "This is normal again. ";
            string part4 = "This is bold text.";
            
            // Объединить все части в одну ячейку
            Cell cell = worksheet.Cells["A1"];
            cell.Value = part1 + part2 + part3 + part4;
            
            // Применить форматирование к определённым частям текста
            int startPos1 = part1.Length;
            int length1 = part2.Length;
            cell.Characters(startPos1, length1).TextOptions.IsBold = true;
            cell.Characters(startPos1, length1).TextOptions.IsItalic = true;
            
            int startPos2 = part1.Length + part2.Length + part3.Length;
            int length2 = part4.Length;
            cell.Characters(startPos2, length2).TextOptions.IsBold = true;
            
            // Сохраните книгу
            workbook.Save("TextOptionsDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("TextOptions demo completed. File saved.");
        }
    }
}
```

### См. также

* class [TextOptions](../../../aspose.cells.drawing.texts/textoptions/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


