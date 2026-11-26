---
title: "Worksheet.Split"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Делит окно"
type: docs
url: /ru/net/aspose.cells/worksheet/split/
---
## Worksheet.Split method

Разделяет окно.

```csharp
public void Split()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSplitDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные для демонстрации разделения
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 1; i <= 50; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Data " + i);
            }
            
            // Разделить лист (параметры не требуются)
            worksheet.Split();
            
            // Сохраните книгу
            workbook.Save("WorksheetSplitDemo.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


