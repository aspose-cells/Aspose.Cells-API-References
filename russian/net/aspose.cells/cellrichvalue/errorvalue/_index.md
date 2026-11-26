---
title: "CellRichValue.ErrorValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellRichValue. Получает тип значения ошибки ячейки"
type: docs
url: /ru/net/aspose.cells/cellrichvalue/errorvalue/
---
## CellRichValue.ErrorValue property

Получает тип значения ошибки ячейки.

```csharp
public virtual ErrorCellValueType ErrorValue { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellRichValuePropertyErrorValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте ошибку переполнения в ячейке A1
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3})";
            
            try
            {
                // Вычислите формулы для создания ошибки переполнения
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // Ожидаемая ошибка spill
            }
            
            // Получите rich value из ячейки A1
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // Проверьте и отобразите тип ошибки
            Console.WriteLine("Error type: " + richValue.ErrorValue);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* enum [ErrorCellValueType](../../errorcellvaluetype/)
* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


