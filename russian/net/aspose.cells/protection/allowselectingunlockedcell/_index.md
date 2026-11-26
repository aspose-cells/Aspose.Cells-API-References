---
title: "Protection.AllowSelectingUnlockedCell"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Представляет, разрешено ли пользователю выбирать разблокированные ячейки на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/allowselectingunlockedcell/
---
## Protection.AllowSelectingUnlockedCell property

Представляет, разрешено ли пользователю выбирать разблокированные ячейки на защищённом листе.

```csharp
public bool AllowSelectingUnlockedCell { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowSelectingUnlockedCellDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Защитите лист со всеми параметрами защиты
            Protection protection = worksheet.Protection;
            
            // Установите AllowSelectingUnlockedCell в значение true
            protection.AllowSelectingUnlockedCell = true;
            protection.AllowSelectingLockedCell = false;
            
            // Примените защиту с паролем
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Проверьте настройку
            Console.WriteLine("AllowSelectingUnlockedCell: " + protection.AllowSelectingUnlockedCell);
            Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);

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


