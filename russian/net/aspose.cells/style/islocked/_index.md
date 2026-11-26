---
title: "Style.IsLocked"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Получает или задает значение, указывающее, может ли ячейка быть изменена"
type: docs
url: /ru/net/aspose.cells/style/islocked/
---
## Style.IsLocked property

Получает или задает значение, указывающее, можно ли изменять ячейку.

```csharp
public bool IsLocked { get; set; }
```

### Примечания

Блокировка ячеек не оказывает эффекта, если лист не защищён.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsLockedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите свойство IsLocked для ячейки
            Cell cell = cells["A1"];
            Style style = cell.GetStyle();
            style.IsLocked = true;
            cell.SetStyle(style);

            // Защитите лист, чтобы применить блокировку
            worksheet.Protect(ProtectionType.All);

            // Проверьте и выведите статус IsLocked
            Console.WriteLine("Cell A1 IsLocked: " + cells["A1"].GetStyle().IsLocked);
            Console.WriteLine("Cell B1 IsLocked: " + cells["B1"].GetStyle().IsLocked);

            // Сохраните книгу
            workbook.Save("IsLockedDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


