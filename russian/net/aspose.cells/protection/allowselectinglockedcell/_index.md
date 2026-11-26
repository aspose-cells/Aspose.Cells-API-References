---
title: "Protection.AllowSelectingLockedCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Представляет, разрешено ли пользователю выбирать защищённые ячейки на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/allowselectinglockedcell/
---
## Protection.AllowSelectingLockedCell property

Представляет, разрешено ли пользователю выбирать заблокированные ячейки на защищённом листе.

```csharp
public bool AllowSelectingLockedCell { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingLockedCellDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установите параметры защиты
            Protection protection = worksheet.Protection;
            
            // Продемонстрировать свойство AllowSelectingLockedCell
            protection.AllowSelectingLockedCell = true;
            Console.WriteLine("AllowSelectingLockedCell is set to: " + protection.AllowSelectingLockedCell);

            // Измените свойство и покажите изменение
            protection.AllowSelectingLockedCell = false;
            Console.WriteLine("AllowSelectingLockedCell is now set to: " + protection.AllowSelectingLockedCell);

            // Защитите лист паролем
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

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


