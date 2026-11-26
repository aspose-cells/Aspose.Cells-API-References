---
title: "ListColumn.GetCustomCalculatedFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListColumn. Получает формулу этого столбца списка"
type: docs
url: /ru/net/aspose.cells.tables/listcolumn/getcustomcalculatedformula/
---
## ListColumn.GetCustomCalculatedFormula method

Получает формулу этого столбца списка.

```csharp
public string GetCustomCalculatedFormula(bool isR1C1, bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isR1C1 | Boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | Boolean | Нужно ли форматировать формулу в соответствии с локалью. |

### Возвращаемое значение

Формула этого столбца списка.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnMethodGetCustomCalculatedFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Создать примерные данные
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B1"].PutValue("Score");
            sheet.Cells["B2"].PutValue(85);
            sheet.Cells["B3"].PutValue(92);
            
            // Создать объект списка
            int index = sheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = sheet.ListObjects[index];
            
            // Добавить вычисляемый столбец
            ListColumn calcColumn = listObject.ListColumns[1];
            calcColumn.Formula = "=WEEKNUM([@Score])";
            
            // Получить пользовательскую вычисляемую формулу
            string formula = listObject.ListColumns[1].GetCustomCalculatedFormula(false, false);
            
            // Вывести результат.
            Console.WriteLine("Calculated Formula: " + formula);
        }
    }
}
```

### См. также

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


