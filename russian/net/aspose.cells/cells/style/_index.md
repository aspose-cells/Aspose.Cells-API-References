---
title: "Cells.Style"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cells. Получает и задает стиль по умолчанию листа"
type: docs
url: /ru/net/aspose.cells/cells/style/
---
## Cells.Style property

Получает и задает стиль по умолчанию листа.

```csharp
public Style Style { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyStyleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите значение в ячейку A1
            Cell cell = cells["A1"];
            cell.PutValue(43368); // This represents the date 2018-09-25

            // Получите стиль по умолчанию и измените его формат
            Style style = cells.Style;
            style.CultureCustom = "yyyymmdd!y";
            
            // Применить изменённый стиль к ячейке
            cell.SetStyle(style);

            // Отобразите отформатированное строковое значение
            Console.WriteLine("Formatted value: " + cell.StringValue);
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


