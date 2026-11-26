---
title: "Перечисление LookInType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.LookInType. Представляет тип поиска"
type: docs
url: /ru/net/aspose.cells/lookintype/
---
## LookInType enumeration

Представляет тип look in.

```csharp
public enum LookInType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Formulas | `0` | Находит искомый объект из формулы([`Formula`](../cell/formula/)), если ячейка содержит формулу, иначе ищет в оригинальном значении ячейки (то же, что OriginalValues). |
| Values | `1` | Находит объект из оригинального значения ячейки([`Value`](../cell/value/)) и форматированного значения([`StringValue`](../cell/stringvalue/)). |
| ValuesExcludeFormulaCell | `2` | Игнорирует ячейки, содержащие формулы. Для ячеек без формул это то же самое, что Values. |
| Comments | `3` | Находит объект только из комментария ячейки. Игнорирует ячейки без комментариев. |
| OnlyFormulas | `4` | Игнорирует ячейки без формул. Для ячеек с формулами ищет искомый объект из формулы([`Formula`](../cell/formula/)). |
| OriginalValues | `5` | Находит объект только из оригинального значения ячейки. |
| FormattedValues | `6` | Находит объект только из форматированного значения ячейки([`StringValue`](../cell/stringvalue/)). |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassLookInTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные и формулы
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].Formula = "=A1";
            worksheet.Cells["C1"].PutValue("Contains B1");

            // Найдите ячейку, содержащую формулу с "B1"
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains
            };

            Cell foundCell = worksheet.Cells.Find("B1", null, options);

            // Вывести результат.
            if (foundCell != null)
            {
                Console.WriteLine($"Found cell at row: {foundCell.Row}, column: {foundCell.Column}");
                Console.WriteLine($"Cell value: {foundCell.StringValue}");
                Console.WriteLine($"Cell formula: {foundCell.Formula}");
            }
            else
            {
                Console.WriteLine("Cell not found");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


