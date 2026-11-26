---
title: "Cells.SetRowHeightInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Устанавливает высоту строки в дюймах"
type: docs
url: /ru/net/aspose.cells/cells/setrowheightinch/
---
## Cells.SetRowHeightInch method

Устанавливает высоту строки в дюймах.

```csharp
public void SetRowHeightInch(int row, double inches)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| дюймы | Double | Количество дюймов. Должно быть от 0 до 409.5/72. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetRowHeightInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить стиль по умолчанию
            Style style = workbook.DefaultStyle;
            style.Font.Name = "Tahoma";
            style.Font.Size = 16;
            style.Font.IsBold = true;
            workbook.DefaultStyle = style;

            // Установить высоту строк в дюймах
            for (int i = 0; i < 10; i++)
            {
                cells.SetRowHeightInch(i, 0.5 + (i * 0.2)); // Demonstrates SetRowHeightInch(Int32, Double)
            }

            // Сохраните книгу
            workbook.Save("RowHeightsInInches.xlsx");
            
            Console.WriteLine("Row heights set successfully in inches.");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


