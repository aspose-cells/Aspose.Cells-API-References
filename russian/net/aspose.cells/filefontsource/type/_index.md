---
title: "FileFontSource.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FileFontSource. Возвращает тип источника шрифта"
type: docs
url: /ru/net/aspose.cells/filefontsource/type/
---
## FileFontSource.Type property

Возвращает тип источника шрифтов.

```csharp
public override FontSourceType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            string fontFilePath = "CustomFont.ttf";
            
            // Создать экземпляр FileFontSource
            FileFontSource fontSource = new FileFontSource(fontFilePath);
            
            // Продемонстрировать использование свойства Type
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            
            // Создать книгу и применить шрифт
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Text with custom font");
            
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont";
            cell.SetStyle(style);
            
            workbook.Save("FontSourceDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FontSourceType](../../fontsourcetype/)
* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


