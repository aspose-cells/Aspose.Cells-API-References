---
title: "Style.IsBorderApplied"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Указывает, следует ли применять форматирование границы"
type: docs
url: /ru/net/aspose.cells/style/isborderapplied/
---
## Style.IsBorderApplied property

Указывает, следует ли применять форматирование границы.

```csharp
public bool IsBorderApplied { get; set; }
```

### Примечания

Только для именованного стиля.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsBorderAppliedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте пользовательский стиль
            Style style = workbook.CreateStyle();
            
            // Примените настройки границы к стилю
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Black;
            
            // Проверьте, применена ли граница
            Console.WriteLine("IsBorderApplied before setting: " + style.IsBorderApplied);
            
            // Явно установить IsBorderApplied в true
            style.IsBorderApplied = true;
            
            // Применить стиль к ячейке
            worksheet.Cells["A1"].SetStyle(style);
            
            // Проверьте применение границы
            Console.WriteLine("IsBorderApplied after setting: " + style.IsBorderApplied);
            
            // Сохраните книгу
            workbook.Save("IsBorderAppliedDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


