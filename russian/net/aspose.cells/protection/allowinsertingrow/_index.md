---
title: "Protection.AllowInsertingRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Указывает, разрешена ли вставка строк на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/allowinsertingrow/
---
## Protection.AllowInsertingRow property

Представляет, разрешено ли вставка строк на защищённом листе

```csharp
public bool AllowInsertingRow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к настройкам защиты
            Protection protection = worksheet.Protection;

            // Разрешить вставку строк при защите
            protection.AllowInsertingRow = true;
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // Попробуйте вставить строку (должно работать, так как AllowInsertingRow равно true)
            worksheet.Cells.InsertRow(0);

            // Сохраните книгу
            workbook.Save("AllowInsertingRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


