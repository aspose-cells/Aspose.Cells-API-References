---
title: "Style.IsProtectionApplied"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Указывает, следует ли применять форматирование защиты"
type: docs
url: /ru/net/aspose.cells/style/isprotectionapplied/
---
## Style.IsProtectionApplied property

Указывает, следует ли применять форматирование защиты.

```csharp
public bool IsProtectionApplied { get; set; }
```

### Примечания

Только для именованного стиля.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsProtectionAppliedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать объект стиля
            Style style = workbook.CreateStyle();
            
            // Установить свойства защиты
            style.IsLocked = true;
            style.IsFormulaHidden = true;
            style.IsProtectionApplied = true;
            
            // Применить стиль к ячейке
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Проверить настройки защиты
            Console.WriteLine("IsProtectionApplied: " + style.IsProtectionApplied);
            Console.WriteLine("IsLocked: " + style.IsLocked);
            Console.WriteLine("IsFormulaHidden: " + style.IsFormulaHidden);
            
            // Изменить настройки защиты
            style.IsProtectionApplied = false;
            Console.WriteLine("\nAfter changing IsProtectionApplied to false:");
            Console.WriteLine("IsProtectionApplied: " + style.IsProtectionApplied);
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


