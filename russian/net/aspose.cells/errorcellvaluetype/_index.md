---
title: "Перечисление ErrorCellValueType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ErrorCellValueType. Представляет значение ячейки, содержащее ошибку"
type: docs
url: /ru/net/aspose.cells/errorcellvaluetype/
---
## ErrorCellValueType enumeration

Представляет значение ячейки, содержащее ошибку.

```csharp
public enum ErrorCellValueType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Value | `1` | Представляет значение ячейки, содержащей ошибку #VALUE!. |
| Ref | `3` | Представляет значение ячейки, содержащей ошибку #REF!. |
| Name | `4` | Представляет значение ячейки, содержащей ошибку #NAME?. |
| NA | `6` | Представляет значение ячейки, содержащей ошибку #N/A. |
| Blocked | `10` | Представляет значение ячейки, содержащей ошибку #BLOCKED!. |
| Busy | `14` | Представляет значение ячейки, содержащей ошибку #BUSY!. |
| Calc | `13` | Представляет значение ячейки, содержащей ошибку #CALC!. |
| Connect | `9` | Представляет значение ячейки, содержащей ошибку #CONNECT!. |
| Field | `12` | Представляет значение ячейки, содержащей ошибку #FIELD!. |
| Spill | `8` | Представляет значение ячейки, содержащей ошибку #SPILL!. |
| Unknown | `11` | Представляет значение ячейки, содержащей ошибку #UNKNOWN!. |
| TimeOut | `19` | Представляет значение ячейки, содержащей ошибку #TIMEOUT!. |
| External | `18` | Представляет значение ячейки, содержащей ошибку #EXTERNAL!. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassErrorCellValueTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите формулу, которая приведёт к ошибке spill
            worksheet.Cells["A1"].Formula = "=UNIQUE({1,2,3;1,2,3})";
            
            try
            {
                // Вычислите формулы, чтобы вызвать ошибку
                workbook.CalculateFormula();
            }
            catch (Exception)
            {
                // Ожидаемая ошибка spill
            }
            
            // Получите расширенное значение ячейки
            CellRichValue richValue = worksheet.Cells["A1"].GetRichValue();
            
            // Проверьте тип ошибки
            if (richValue.ErrorValue == ErrorCellValueType.Spill)
            {
                Console.WriteLine("Cell contains a spill error as expected");
            }
            
            // Сохраните книгу
            workbook.Save("ErrorCellValueTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


