---
title: "Worksheet.Protection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Представляет различные типы параметров защиты, доступные для листа. Поддерживает расширенные параметры защиты в ExcelXP и более новых версиях"
type: docs
url: /ru/net/aspose.cells/worksheet/protection/
---
## Worksheet.Protection property

Представляет различные типы параметров защиты, доступных для листа. Поддерживает расширенные параметры защиты в ExcelXP и более новых версиях.

```csharp
public Protection Protection { get; }
```

### Примечания

Это свойство может защищать лист во всех версиях файлов Excel и поддерживает расширенные параметры защиты в ExcelXP и более новых версиях.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyProtectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Доступ к свойствам защиты
            Protection protection = sheet.Protection;
            
            // Установить свойства защиты
            protection.AllowEditingObject = false;
            protection.AllowEditingScenario = false;
            
            // Защитить лист (используя метод Protect вместо прямой установки IsProtectedWithPassword)
            sheet.Protect(ProtectionType.All, "password123", null);

            // Сохраните книгу
            workbook.Save("WorksheetProtectionDemo.xlsx");

            // Проверить настройки защиты
            Console.WriteLine("AllowEditingObject: " + protection.AllowEditingObject);
            Console.WriteLine("AllowEditingScenario: " + protection.AllowEditingScenario);
        }
    }
}
```

### См. также

* class [Protection](../../protection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


