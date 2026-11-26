---
title: "Protection.AllowInsertingColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Указывает, разрешена ли вставка столбцов на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/allowinsertingcolumn/
---
## Protection.AllowInsertingColumn property

Представляет, разрешено ли вставка столбцов на защищённом листе

```csharp
public bool AllowInsertingColumn { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получите настройки защиты
            Protection protection = worksheet.Protection;

            // Установите AllowInsertingColumn в true
            protection.AllowInsertingColumn = true;

            // Проверьте настройку
            Console.WriteLine("AllowInsertingColumn is set to: " + protection.AllowInsertingColumn);

            // Защитите лист паролем (используя метод Workbook.Protect)
            workbook.Protect(ProtectionType.All, "password123");
            protection.AllowInsertingColumn = true; // Explicitly set again to demonstrate

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


