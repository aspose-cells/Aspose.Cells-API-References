---
title: "FontSetting.Length"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FontSetting. Получает длину символов"
type: docs
url: /ru/net/aspose.cells/fontsetting/length/
---
## FontSetting.Length property

Получает длину символов.

```csharp
public int Length { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyLengthDemo
    {
        public static void Run()
        {
            // Создайте книгу и получите доступ к её первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторый текст в ячейку A1
            worksheet.Cells["A1"].PutValue("Hello World");

            // Создайте настройки шрифта для текста в ячейке A1
            FontSetting fontSetting = worksheet.Cells["A1"].Characters(0, 5);
            
            // Продемонстрируйте использование свойства Length
            Console.WriteLine("Original Length: " + fontSetting.Length);
            
            // Измените длину настройки шрифта
            fontSetting = worksheet.Cells["A1"].Characters(0, 11);
            Console.WriteLine("Modified Length: " + fontSetting.Length);
            
            // Примените форматирование к настройке шрифта
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // Сохраните книгу
            workbook.Save("FontSettingLengthDemo.xlsx");
        }
    }
}
```

### См. также

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


