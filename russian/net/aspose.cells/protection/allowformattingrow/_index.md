---
title: "Protection.AllowFormattingRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Указывает, разрешено ли форматирование строк на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/allowformattingrow/
---
## Protection.AllowFormattingRow property

Представляет, разрешено ли форматирование строк на защищённом листе

```csharp
public bool AllowFormattingRow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Включить защиту листа
            worksheet.Protect(ProtectionType.All);

            // Доступ к настройкам защиты
            Protection protection = worksheet.Protection;

            // Разрешить форматирование строк, сохраняя остальные защиты
            protection.AllowFormattingRow = true;

            // Сохраните книгу
            workbook.Save("Protection_AllowFormattingRow.xlsx");
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


