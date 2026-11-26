---
title: "ListColumn.SetCustomTotalsRowFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ListColumn. Получает формулу строки итогов этого столбца списка"
type: docs
url: /ru/net/aspose.cells.tables/listcolumn/setcustomtotalsrowformula/
---
## ListColumn.SetCustomTotalsRowFormula method

Получает формулу строки итогов этого столбца списка.

```csharp
public void SetCustomTotalsRowFormula(string formula, bool isR1C1, bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | формула для этого столбца списка. |
| isR1C1 | Boolean | Нужно ли форматировать формулу как R1C1. |
| isLocal | Boolean | Нужно ли форматировать формулу в соответствии с локалью. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnMethodSetCustomTotalsRowFormulaWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные в лист
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);

            // Создать объект списка
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Включить строку итогов и задать пользовательскую формулу
            listObject.ShowTotals = true;
            listObject.ListColumns[0].TotalsCalculation = TotalsCalculation.Custom;
            listObject.ListColumns[0].SetCustomTotalsRowFormula("=SUM([Column1])", false, false);

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


