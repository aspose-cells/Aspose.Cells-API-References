---
title: "Worksheet.IsProtected"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Указывает, защищён ли лист"
type: docs
url: /ru/net/aspose.cells/worksheet/isprotected/
---
## Worksheet.IsProtected property

Указывает, защищён ли лист.

```csharp
public bool IsProtected { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsProtectedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Защитите книгу и первый лист
            workbook.Protect(ProtectionType.All, "password");
            workbook.Worksheets[0].Protect(ProtectionType.All, "password", null);

            // Проверьте, защищён ли рабочий лист
            bool isProtected = workbook.Worksheets[0].IsProtected;
            Console.WriteLine($"Worksheet is protected: {isProtected}");

            // Сохраните книгу
            workbook.Save("protected_worksheet.xlsx");

            // Загрузите сохранённую книгу и проверьте защиту
            Workbook loadedWorkbook = new Workbook("protected_worksheet.xlsx");
            Console.WriteLine($"Loaded worksheet is protected: {loadedWorkbook.Worksheets[0].IsProtected}");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


