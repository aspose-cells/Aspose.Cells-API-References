---
title: "Style.IsPercent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Указывает, является ли числовой формат процентным"
type: docs
url: /ru/net/aspose.cells/style/ispercent/
---
## Style.IsPercent property

Указывает, является ли числовой формат процентным.

```csharp
public bool IsPercent { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StylePropertyIsPercentDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить доступ к ячейке A1 и установить её значение
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(0.5);
            
            // Получить стиль ячейки
            Style style = cell.GetStyle();
            
            // Отобразить текущее значение IsPercent
            Console.WriteLine("Current IsPercent value: " + style.IsPercent);
            
            // Установить числовой формат в процентный (это автоматически установит IsPercent в true)
            style.Number = 10; // 10 is the built-in percentage format in Excel
            
            // Применить стиль к ячейке
            cell.SetStyle(style);
            
            // Проверьте, что IsPercent теперь true
            Console.WriteLine("After setting percentage format, IsPercent value: " + style.IsPercent);
            
            // Создайте другую ячейку с другим форматом
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue(0.75);
            Style style2 = cell2.GetStyle();
            style2.Number = 3; // 3 is the built-in number format (not percentage)
            cell2.SetStyle(style2);
            
            // Проверьте, что IsPercent равно false для формата, не являющегося процентом
            Console.WriteLine("For non-percentage format, IsPercent value: " + style2.IsPercent);
            
            // Сохраните книгу
            workbook.Save("StylePropertyIsPercentDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


