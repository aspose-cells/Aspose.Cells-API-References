---
title: "Style.ToJson"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Style. Преобразовать Style в структуру данных JSON"
type: docs
url: /ru/net/aspose.cells/style/tojson/
---
## Style.ToJson method

Преобразовать [`Style`](../) в структуру данных JSON.

```csharp
public string ToJson()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodToJsonDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать и применить стиль к ячейке B4
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Yellow;
            cells["B4"].SetStyle(style);

            // Преобразовать стиль в JSON
            string styleJson = style.ToJson();
            Console.WriteLine("Style JSON:");
            Console.WriteLine(styleJson);

            // Установите формулу в ячейку B6
            cells["B6"].Formula = "=A1";

            // Преобразовать ячейку в JSON
            string cellJson = cells["B6"].ToJson();
            Console.WriteLine("\nCell JSON:");
            Console.WriteLine(cellJson);
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


