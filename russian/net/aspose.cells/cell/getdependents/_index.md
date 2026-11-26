---
title: "Cell.GetDependents"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Получить все ячейки, формулы которых напрямую ссылаются на эту ячейку"
type: docs
url: /ru/net/aspose.cells/cell/getdependents/
---
## Cell.GetDependents method

Получить все ячейки, формула которых напрямую ссылается на эту ячейку.

```csharp
public Cell[] GetDependents(bool isAll)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| isAll | Boolean | Указывает, следует ли проверять формулы в других листах |

### Примечания

Если ссылка, содержащая эту ячейку, появляется в формуле какой‑то ячейки, эта ячейка будет считаться зависимой от данной ячейки, независимо от того, используется ссылка или данная ячейка при вычислении. Например, хотя ячейка A2 в формуле "=IF(TRUE,A1,A2)" не используется при вычислении, эта формула всё равно считается зависимой от A2. Чтобы получить формулы, результаты вычисления которых зависят от этой ячейки, используйте [`GetDependentsInCalculation`](../getdependentsincalculation/). При трассировке зависимых для одной ячейки все формулы в книге или листе будут проанализированы и проверены. Поэтому процесс занимает много времени. Если пользователю нужно трассировать зависимые для большого количества ячеек, использование этого метода приведёт к плохой производительности. С учётом производительности следует использовать [`GetDependentsInCalculation`](../getdependentsincalculation/) вместо него. Либо пользователь может сначала собрать карту предшествующих ячеек для всех ячеек с помощью [`GetPrecedents`](../getprecedents/), а затем построить карту зависимых на основе карты предшествующих.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установите формулы, которые ссылаются на B1
            cells["A1"].Formula = "=B1+5";
            cells["A2"].Formula = "=B1*2";
            cells["A3"].Formula = "=SUM(B1:B3)";

            // Вычислить формулы
            workbook.CalculateFormula();

            // Получите все ячейки, зависящие от B1 (рекурсивно)
            Cell[] dependents = cells["B1"].GetDependents(true);

            Console.WriteLine("Cells dependent on B1:");
            foreach (Cell cell in dependents)
            {
                Console.WriteLine(cell.Name + ": " + cell.Formula);
            }
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


