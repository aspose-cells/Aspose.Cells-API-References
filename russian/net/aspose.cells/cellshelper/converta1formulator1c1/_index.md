---
title: "CellsHelper.ConvertA1FormulaToR1C1"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Преобразует формулу A1 ячейки в формулу r1c1."
type: docs
url: /ru/net/aspose.cells/cellshelper/converta1formulator1c1/
---
## CellsHelper.ConvertA1FormulaToR1C1 method

Преобразует формулу A1 ячейки в формулу r1c1.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertA1FormulaToR1C1(string formula, int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Формула A1. |
| строка | Int32 | Индекс строки ячейки. |
| column | Int32 | Индекс столбца ячейки. |

### Возвращаемое значение

Формула R1C1.

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо него, пожалуйста, используйте метод Worksheet.ConvertFormulaReferenceStyle(). Это свойство будет удалено через 12 месяцев, начиная с августа 2023 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodConvertA1FormulaToR1C1WithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Преобразовать формулу в стиле A1 в стиль R1C1
            string r1c1Formula = CellsHelper.ConvertA1FormulaToR1C1("=A1+B2", 0, 0);
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
        }
    }
}
```

### См. также

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


