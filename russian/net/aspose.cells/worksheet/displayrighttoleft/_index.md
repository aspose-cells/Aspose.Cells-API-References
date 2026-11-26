---
title: "Worksheet.DisplayRightToLeft"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Указывает, отображается ли указанный лист справа налево вместо слева направо. По умолчанию — false"
type: docs
url: /ru/net/aspose.cells/worksheet/displayrighttoleft/
---
## Worksheet.DisplayRightToLeft property

Указывает, отображается ли указанный лист справа налево вместо слева направо. По умолчанию false.

```csharp
public bool DisplayRightToLeft { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyDisplayRightToLeftDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите отображение справа налево
            worksheet.DisplayRightToLeft = true;
            
            // Сохраните книгу
            workbook.Save("output.ods");
            
            // Перезагрузите книгу, чтобы проверить настройку
            Workbook loadedWorkbook = new Workbook("output.ods");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            Console.WriteLine("DisplayRightToLeft: " + loadedWorksheet.DisplayRightToLeft);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


