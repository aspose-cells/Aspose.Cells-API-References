---
title: "Font.IsSuperscript"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Font. Получает или задает значение, указывающее, является ли шрифт надстрочным"
type: docs
url: /ru/net/aspose.cells/font/issuperscript/
---
## Font.IsSuperscript property

Получает или задает значение, указывающее, является ли шрифт верхним индексом.

```csharp
public bool IsSuperscript { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSuperscriptDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить текст в ячейку A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Normal Text Superscript Text");
            
            // Отформатировать часть текста как надстрочный
            FontSetting setting = cell.Characters(12, 11);
            setting.Font.IsSuperscript = true;
            
            // Сохраните книгу
            workbook.Save("FontIsSuperscriptDemo.xlsx");
            
            // Проверьте настройку надстрочного текста
            Console.WriteLine("IsSuperscript property: " + setting.Font.IsSuperscript);
        }
    }
}
```

### См. также

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


