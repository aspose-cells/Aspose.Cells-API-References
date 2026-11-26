---
title: "Cell.ToJson"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Преобразовать Cell в структуру данных JSON"
type: docs
url: /ru/net/aspose.cells/cell/tojson/
---
## Cell.ToJson method

Преобразовать [`Cell`](../) в структуру данных JSON.

```csharp
public string ToJson()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodToJsonDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите примерные данные и стили
            cells["A1"].PutValue(100);
            cells["B6"].Formula = "=A1";
            
            // Получите ячейку и преобразуйте в JSON
            Cell cell = cells["B6"];
            string json = cell.ToJson();
            
            // Вывести JSON
            Console.WriteLine("Cell JSON:");
            Console.WriteLine(json);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


