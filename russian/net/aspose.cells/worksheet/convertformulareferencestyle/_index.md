---
title: "Worksheet.ConvertFormulaReferenceStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Преобразует стиль ссылок формулы"
type: docs
url: /ru/net/aspose.cells/worksheet/convertformulareferencestyle/
---
## Worksheet.ConvertFormulaReferenceStyle method

Преобразует стиль ссылок в формуле.

```csharp
public string ConvertFormulaReferenceStyle(string formula, bool toR1C1, int baseCellRow, 
    int baseCellColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Формула, которую нужно преобразовать. |
| toR1C1 | Boolean | Стиль ссылки, в который следует преобразовать формулу. Если исходная формула использует стиль ссылок A1, то это значение должно быть true, чтобы формула была преобразована из стиля A1 в R1C1; если исходная формула использует стиль R1C1, то это значение должно быть false, чтобы формула была преобразована из стиля R1C1 в A1; |
| baseCellRow | Int32 | Индекс строки базовой ячейки. |
| baseCellColumn | Int32 | Индекс столбца базовой ячейки. |

### Возвращаемое значение

Преобразованная формула.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodConvertFormulaReferenceStyleWithStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Пример 1: Преобразовать стиль R1C1 в стиль A1
            string formulaR1C1 = "R[0]C23,testDS,R[0]C24";
            string formulaA1 = sheet.ConvertFormulaReferenceStyle(formulaR1C1, false, 0, 0);
            Console.WriteLine("Converted formula: " + formulaA1);

            // Пример 2: Преобразовать с смешанными ссылками
            string formulaMixed = "R[0]C23,testDS,rcurr,R[0]C24";
            string convertedMixed = sheet.ConvertFormulaReferenceStyle(formulaMixed, false, 0, 0);
            Console.WriteLine("Converted mixed formula: " + convertedMixed);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


