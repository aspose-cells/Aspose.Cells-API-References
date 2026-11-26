---
title: "Worksheet.IsPageBreakPreview"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Указывает, отображается ли указанный лист в обычном виде или в режиме предварительного просмотра разрывов страниц"
type: docs
url: /ru/net/aspose.cells/worksheet/ispagebreakpreview/
---
## Worksheet.IsPageBreakPreview property

Указывает, отображается ли указанный лист в обычном виде или в режиме предварительного просмотра разрывов страниц.

```csharp
public bool IsPageBreakPreview { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsPageBreakPreviewDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите лист в режим предварительного просмотра разрывов страниц
            worksheet.IsPageBreakPreview = true;
            
            // Установите масштаб 100 % для демонстрации
            worksheet.Zoom = 100;
            
            // Выведите текущие настройки
            Console.WriteLine("IsPageBreakPreview: " + worksheet.IsPageBreakPreview);
            Console.WriteLine("Zoom: " + worksheet.Zoom);
            
            // Сохраните книгу
            workbook.Save("WorksheetPropertyIsPageBreakPreviewDemo_output.xlsx");
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


