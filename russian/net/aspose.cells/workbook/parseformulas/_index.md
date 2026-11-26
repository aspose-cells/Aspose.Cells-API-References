---
title: "Workbook.ParseFormulas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Разбирает все формулы, которые не были разобраны при загрузке из шаблона или при установке в ячейку"
type: docs
url: /ru/net/aspose.cells/workbook/parseformulas/
---
## Workbook.ParseFormulas method

Разбирает все формулы, которые не были разобраны при загрузке из шаблонного файла или при установке в ячейку.

```csharp
public void ParseFormulas(bool ignoreError)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ignoreError | Boolean | Нужно ли игнорировать ошибку для неверной формулы. Для одной неверной формулы, если игнорировать ошибку, то эта формула будет пропущена и процесс продолжит разбор остальных формул, иначе будет выброшено исключение. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodParseFormulasWithBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить формулы без разбора (Parse = false)
            for (int i = 1; i < 10; i++)
            {
                cells[i, 0].SetFormula($"=SUM(A{i}:B{i})", new FormulaParseOptions() { Parse = false }, null);
            }

            Console.WriteLine("Formulas set without parsing. Now parsing them all at once...");

            // Разобрать все формулы сразу
            wb.ParseFormulas(false);

            // Проверить формулы
            for (int i = 1; i < 10; i++)
            {
                Console.WriteLine($"Cell A{i} formula: {cells[i, 0].Formula}");
            }
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


