---
title: "Font.Color"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Font. Получает или задает цвет шрифта"
type: docs
url: /ru/net/aspose.cells/font/color/
---
## Font.Color property

Получает или задаёт цвет шрифта.

```csharp
public Color Color { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FontPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите HTML с разными цветами шрифта и стилями
            Cell cell = worksheet.Cells["A1"];
            cell.HtmlString = "<font color='Red'>Red Text</font> <font color='#0000FF'>Blue Text</font><font style='color:#00FF00;text-decoration: underline;'>Green Underlined</font>";
            
            // Получите форматирование богатого текста
            FontSetting[] richText = cell.GetCharacters();
            
            // Проверьте и продемонстрируйте свойства цвета
            Console.WriteLine("First segment color: " + richText[0].Font.Color);
            Console.WriteLine("Second segment color: " + richText[1].Font.Color);
            Console.WriteLine("Third segment underline: " + richText[2].Font.Underline);
            
            // Сохраните книгу
            workbook.Save("FontColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


