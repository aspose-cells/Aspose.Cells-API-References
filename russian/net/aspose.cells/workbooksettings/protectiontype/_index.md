---
title: "WorkbookSettings.ProtectionType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorkbookSettings. Возвращает тип защиты книги"
type: docs
url: /ru/net/aspose.cells/workbooksettings/protectiontype/
---
## WorkbookSettings.ProtectionType property

Получает тип защиты книги.

```csharp
public ProtectionType ProtectionType { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyProtectionTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Защитите книгу с типом защиты Windows
            workbook.Protect(ProtectionType.Windows, "password123");
            
            // Продемонстрируйте свойство ProtectionType
            Console.WriteLine("Workbook protection type: " + workbook.Settings.ProtectionType);
            
            // Сохраните книгу
            workbook.Save("ProtectedWorkbook.xlsx");
            
            // Загрузите сохранённую книгу, чтобы проверить, сохраняется ли тип защиты
            Workbook loadedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            Console.WriteLine("Loaded workbook protection type: " + loadedWorkbook.Settings.ProtectionType);
        }
    }
}
```

### См. также

* enum [ProtectionType](../../protectiontype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


