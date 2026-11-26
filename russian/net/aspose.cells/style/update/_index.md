---
title: "Style.Update"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Style. Применить именованный стиль к стилям ячеек, использующих этот именованный стиль. Это работает как нажатие кнопки OK после завершения изменения стиля. Применяется только к именованному стилю"
type: docs
url: /ru/net/aspose.cells/style/update/
---
## Style.Update method

Применить именованный стиль к стилям ячеек, использующих этот именованный стиль. Это работает как нажатие кнопки "ok" после завершения изменения стиля. Применяется только к именованному стилю.

```csharp
public void Update()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodUpdateDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать стиль
            Style style = workbook.CreateStyle();
            style.Number = 3; // Set to Percent format
            
            // Применить стиль к ячейке A1
            worksheet.Cells["A1"].SetStyle(style);
            
            // Изменить стиль
            style.Number = 4; // Change to Currency format
            
            // Обновить изменения стиля
            style.Update();
            
            // Проверить, что стиль был обновлён
            Console.WriteLine("Cell A1 Number Format: " + worksheet.Cells["A1"].GetStyle().Number);
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


