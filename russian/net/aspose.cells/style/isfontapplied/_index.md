---
title: "Style.IsFontApplied"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Укажите, следует ли применять форматирование шрифта"
type: docs
url: /ru/net/aspose.cells/style/isfontapplied/
---
## Style.IsFontApplied property

Указывает, следует ли применять форматирование шрифта.

```csharp
public bool IsFontApplied { get; set; }
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
    public class StylePropertyIsFontAppliedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к ячейке листа
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            
            // Получить стиль ячейки
            Style style = cell.GetStyle();
            
            // Применить настройки шрифта
            style.Font.Name = "Times New Roman";
            style.Font.Size = 14;
            style.Font.Color = Color.Blue;
            
            // Включить применение шрифта
            style.IsFontApplied = true;
            
            // Установите изменённый стиль обратно в ячейку
            cell.SetStyle(style);
            
            // Сохраните книгу
            workbook.Save("FontAppliedDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


