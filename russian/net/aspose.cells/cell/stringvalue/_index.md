---
title: "Cell.StringValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Cell. Возвращает строковое значение, содержащееся в ячейке. Если тип этой ячейки — строка, то возвращается само строковое значение. Для остальных типов ячеек будет возвращено отформатированное строковое значение, отформатированное согласно указанному стилю этой ячейки. Отформатированное значение ячейки совпадает с тем, что можно получить из Excel при копировании ячейки как текста, например при копировании ячейки в текстовый редактор или экспорте в CSV."
type: docs
url: /ru/net/aspose.cells/cell/stringvalue/
---
## Cell.StringValue property

Получает строковое значение, содержащееся в ячейке. Если тип этой ячейки — строка, возвращается само строковое значение. Для остальных типов ячеек будет возвращено отформатированное строковое значение (отформатированное с использованием указанного стиля этой ячейки). Отформатированное значение ячейки совпадает с тем, что можно получить из Excel при копировании ячейки как текста (например, при копировании ячейки в текстовый редактор или экспорте в CSV).

```csharp
public string StringValue { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyStringValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить некоторые значения
            cells["A1"].PutValue("Hello");
            cells["A2"].PutValue(123);
            cells["A3"].PutValue(DateTime.Now);
            cells["A4"].Formula = "=A1&A2";

            // Вычислить формулы
            workbook.CalculateFormula();

            // Продемонстрировать свойство StringValue
            Console.WriteLine("A1 StringValue: " + cells["A1"].StringValue);
            Console.WriteLine("A2 StringValue: " + cells["A2"].StringValue);
            Console.WriteLine("A3 StringValue: " + cells["A3"].StringValue);
            Console.WriteLine("A4 StringValue: " + cells["A4"].StringValue);

            // Показать случай значения ошибки
            Cell errorCell = cells["B1"];
            errorCell.Formula = "=1/0";
            workbook.CalculateFormula();
            Console.WriteLine("B1 (Error) StringValue: " + errorCell.StringValue);
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


