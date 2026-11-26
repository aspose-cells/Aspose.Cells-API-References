---
title: "Style.IsFillApplied"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Указывает, следует ли применять форматирование заливки"
type: docs
url: /ru/net/aspose.cells/style/isfillapplied/
---
## Style.IsFillApplied property

Указывает, следует ли применять форматирование заливки.

```csharp
public bool IsFillApplied { get; set; }
```

### Примечания

Только для именованного стиля.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFillAppliedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать стиль
            Style style = workbook.CreateStyle();
            
            // Изначально IsFillApplied должно быть false
            Console.WriteLine("IsFillApplied (initial): " + style.IsFillApplied);
            
            // Применить настройки заливки
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // После установки свойств заливки IsFillApplied должно быть true
            Console.WriteLine("IsFillApplied (after setting fill): " + style.IsFillApplied);
            
            // Применить стиль к ячейке
            worksheet.Cells["A1"].SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("IsFillAppliedDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


