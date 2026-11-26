---
title: "Style.IsJustifyDistributed"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Style property. Указывает, следует ли использовать выравнивание по ширине или распределённое выравнивание для последней строки текста"
type: docs
url: /ru/net/aspose.cells/style/isjustifydistributed/
---
## Style.IsJustifyDistributed property

Указывает, следует ли использовать выравнивание по ширине или распределённое выравнивание ячеек в последней строке текста.

```csharp
public bool IsJustifyDistributed { get; set; }
```

### Примечания

Это типично для восточноазиатских выравниваний, но не типично в других контекстах. Работает только при распределённом горизонтальном выравнивании.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsJustifyDistributedDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к ячейке B3 и установить её текст
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("Sample Text");

            // Получить стиль ячейки и установить IsJustifyDistributed в true
            Style style = cell.GetStyle();
            style.IsJustifyDistributed = true;
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("output.xlsx");

            // Проверить свойство
            Console.WriteLine("IsJustifyDistributed: " + cell.GetStyle().IsJustifyDistributed);
        }
    }
}
```

### См. также

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


