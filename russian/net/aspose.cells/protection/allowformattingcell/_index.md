---
title: "Protection.AllowFormattingCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Представляет, разрешено ли форматирование ячеек на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/allowformattingcell/
---
## Protection.AllowFormattingCell property

Представляет, разрешено ли форматирование ячеек на защищённом листе.

```csharp
public bool AllowFormattingCell { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingCellDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Включить защиту листа
            Protection protection = worksheet.Protection;
            
            // Установите различные свойства защиты, используя флаг
            int flag = 0x40; // Only AllowFormattingCell flag is set
            protection.AllowFormattingCell = (flag & 0x40) != 0;

            // Проверьте настройку
            Console.WriteLine("AllowFormattingCell is set to: " + protection.AllowFormattingCell);

            // Сохраните книгу
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


