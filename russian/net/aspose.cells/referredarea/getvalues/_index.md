---
title: "ReferredArea.GetValues"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ReferredArea. Получает значения ячеек в этой области"
type: docs
url: /ru/net/aspose.cells/referredarea/getvalues/
---
## GetValues() {#getvalues}

Получает значения ячеек в этой области.

```csharp
public object GetValues()
```

### Возвращаемое значение

Если эта область недействительна, будет возвращено "#REF!"; если область состоит из одной ячейки, будет возвращён объект значения ячейки; в противном случае будет возвращён двумерный массив со всеми значениями в этой области.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Collections;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["B1"].PutValue(3);
            worksheet.Cells["B2"].PutValue(4);

            Cell formulaCell = worksheet.Cells["C1"];
            formulaCell.Formula = "=SUM(A1:B2)";

            ReferredAreaCollection referredAreas = formulaCell.GetPrecedents();
            if (referredAreas.Count > 0)
            {
                ReferredArea ra = referredAreas[0];
                object vs = ra.GetValues();

                if (vs is Array)
                {
                    object[][] values = (object[][])vs;
                    foreach (object[] row in values)
                    {
                        foreach (object val in row)
                        {
                            Console.WriteLine($"Value: {val}");
                        }
                    }
                }
            }
        }
    }
}
```

### См. также

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetValues(bool) {#getvalues_1}

Получает значения ячеек в этой области.

```csharp
public object GetValues(bool calculateFormulas)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| calculateFormulas | Boolean | В этом диапазоне, если есть формулы, которые не были вычислены, этот флаг указывает, следует ли вычислять эти формулы рекурсивно. |

### Возвращаемое значение

Если эта область недействительна, будет возвращено "#REF!"; если область состоит из одной ячейки, будет возвращён объект значения ячейки; в противном случае будет возвращён двумерный массив со всеми значениями в этой области.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaMethodGetValuesWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            string formula = "=A1:B2";
            Cell cell = worksheet.Cells["C1"];
            cell.Formula = formula;

            workbook.CalculateFormula();
            
            ReferredAreaCollection referredAreasCollection = cell.GetPrecedents();
            ReferredArea[] referredAreas = new ReferredArea[referredAreasCollection.Count];
            for (int i = 0; i < referredAreasCollection.Count; i++)
            {
                referredAreas[i] = referredAreasCollection[i];
            }

            if (referredAreas.Length > 0)
            {
                ReferredArea ra = referredAreas[0];
                
                Console.WriteLine("With headers (true):");
                PrintResult(ra.GetValues(true));
                
                Console.WriteLine("\nWithout headers (false):");
                PrintResult(ra.GetValues(false));
            }
        }

        private static void PrintResult(object result)
        {
            if (result is object[,] multiArray)
            {
                for (int i = 0; i < multiArray.GetLength(0); i++)
                {
                    for (int j = 0; j < multiArray.GetLength(1); j++)
                    {
                        Console.Write(multiArray[i, j] + "\t");
                    }
                    Console.WriteLine();
                }
            }
            else if (result is object[] singleArray)
            {
                Console.WriteLine(string.Join("\t", singleArray));
            }
            else
            {
                Console.WriteLine(result);
            }
        }
    }
}
```

### См. также

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


