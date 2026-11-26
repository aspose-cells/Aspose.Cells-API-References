---
title: "ListColumn.GetCustomTotalsRowFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListColumn. Получает формулу строки итогов этого столбца списка"
type: docs
url: /ru/net/aspose.cells.tables/listcolumn/getcustomtotalsrowformula/
---
## ListColumn.GetCustomTotalsRowFormula method

Получает формулу строки итогов этого столбца списка.

```csharp
public string GetCustomTotalsRowFormula(bool isR1C1, bool isLocal)
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
    public class ListColumnMethodGetCustomTotalsRowFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);

            // Создать объект списка
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Задать пользовательскую формулу итогов
            ListColumn listColumn = listObject.ListColumns[0];
            listColumn.TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Custom;
            listColumn.SetCustomTotalsRowFormula("=SUM([Column1])", false, false);

            // Получить и отобразить пользовательскую формулу итогов
            string formula = listColumn.GetCustomTotalsRowFormula(false, true);
            Console.WriteLine("Custom Totals Formula: " + formula);

            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


