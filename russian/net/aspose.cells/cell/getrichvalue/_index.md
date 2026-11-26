---
title: "Cell.GetRichValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получает расширенное значение ячейки"
type: docs
url: /ru/net/aspose.cells/cell/getrichvalue/
---
## Cell.GetRichValue method

Получает расширенное значение ячейки.

```csharp
public CellRichValue GetRichValue()
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetRichValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet ws = wb.Worksheets[0];
            
            // Установите значение rich text в ячейку A1
            ws.Cells["A1"].PutValue("This is rich text");
            
            // Получить расширенное значение из ячейки A1
            CellRichValue richValue = ws.Cells["A1"].GetRichValue();
            
            // Отобразите значение rich text
            Console.WriteLine("Rich Text Value: " + ws.Cells["A1"].StringValue);
            
            // Сохраните книгу
            wb.Save("RichValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [CellRichValue](../../cellrichvalue/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


