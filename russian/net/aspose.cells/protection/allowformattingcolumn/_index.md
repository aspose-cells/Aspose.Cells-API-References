---
title: "Protection.AllowFormattingColumn"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Protection. Указывает, разрешено ли форматирование столбцов на защищённом листе"
type: docs
url: /ru/net/aspose.cells/protection/allowformattingcolumn/
---
## Protection.AllowFormattingColumn property

Представляет, разрешено ли форматирование столбцов на защищённом листе

```csharp
public bool AllowFormattingColumn { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingColumnDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Доступ к настройкам защиты
            Protection protection = worksheet.Protection;

            // Установить свойство AllowFormattingColumn
            protection.AllowFormattingColumn = true;

            // Проверить и вывести значение свойства
            Console.WriteLine("AllowFormattingColumn: " + protection.AllowFormattingColumn);

            // Продемонстрировать установку нескольких свойств защиты
            protection.AllowDeletingColumn = true;
            protection.AllowFormattingRow = true;

            // Вызвать метод вычисления флага
            int protectionFlags = CalculateProtectionFlags(protection);
            Console.WriteLine("Protection Flags: 0x" + protectionFlags.ToString("X4"));
        }

        private static int CalculateProtectionFlags(Protection protection)
        {
            int flag = 0;
            if (protection.AllowDeletingColumn) { flag |= 0x0001; }
            if (protection.AllowDeletingRow) { flag |= 0x0002; }
            if (protection.AllowEditingContent) { flag |= 0x0004; }
            if (protection.AllowEditingObject) { flag |= 0x0008; }
            if (protection.AllowEditingScenario) { flag |= 0x0010; }
            if (protection.AllowFiltering) { flag |= 0x0020; }
            if (protection.AllowFormattingCell) { flag |= 0x0040; }
            if (protection.AllowFormattingColumn) { flag |= 0x0080; }
            if (protection.AllowFormattingRow) { flag |= 0x0100; }
            if (protection.AllowInsertingColumn) { flag |= 0x0200; }
            if (protection.AllowInsertingHyperlink) { flag |= 0x0400; }
            if (protection.AllowInsertingRow) { flag |= 0x0800; }
            if (protection.AllowSelectingLockedCell) { flag |= 0x1000; }
            if (protection.AllowSelectingUnlockedCell) { flag |= 0x2000; }
            if (protection.AllowSorting) { flag |= 0x4000; }
            if (protection.AllowUsingPivotTable) { flag |= 0x8000; }
            return flag;
        }
    }
}
```

### См. также

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


