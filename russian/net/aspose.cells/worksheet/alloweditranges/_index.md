---
title: "Worksheet.AllowEditRanges"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Получает коллекцию разрешённых диапазонов редактирования в листе"
type: docs
url: /ru/net/aspose.cells/worksheet/alloweditranges/
---
## Worksheet.AllowEditRanges property

Получает коллекцию разрешённых диапазонов редактирования в рабочем листе.

```csharp
public ProtectedRangeCollection AllowEditRanges { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAllowEditRangesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить разрешённый диапазон редактирования
            int index = worksheet.AllowEditRanges.Add("r1", 0, 0, 1, 1);
            ProtectedRange range = worksheet.AllowEditRanges[index];
            range.Password = "password123";

            // Защитить лист
            worksheet.Protect(ProtectionType.All);

            // Сохраните книгу
            workbook.Save("output.xlsx");

            // Загрузите сохранённую книгу для проверки
            Workbook verifyWorkbook = new Workbook("output.xlsx");
            ProtectedRange verifyRange = verifyWorkbook.Worksheets[0].AllowEditRanges[0];
            Console.WriteLine("Is protected with password: " + verifyRange.IsProtectedWithPassword);
        }
    }
}
```

### См. также

* class [ProtectedRangeCollection](../../protectedrangecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


