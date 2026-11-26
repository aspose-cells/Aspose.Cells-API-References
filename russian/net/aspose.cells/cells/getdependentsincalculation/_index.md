---
title: "Cells.GetDependentsInCalculation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Получает все ячейки, результат расчёта которых зависит от конкретной ячейки"
type: docs
url: /ru/net/aspose.cells/cells/getdependentsincalculation/
---
## Cells.GetDependentsInCalculation method

Получает все ячейки, результат вычисления которых зависит от конкретной ячейки.

```csharp
public IEnumerator GetDependentsInCalculation(int row, int column, bool recursive)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки конкретной ячейки |
| column | Int32 | Индекс столбца конкретной ячейки. |
| recursive | Boolean | Возвращает те зависимые элементы, которые не ссылаются напрямую на конкретную ячейку, а ссылаются на другие листовые элементы этой ячейки. |

### Возвращаемое значение

Перечислитель для перечисления всех зависимых (объекты Cell)

### Примечания

Чтобы использовать этот метод, убедитесь, что для рабочей книги установлен параметр [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) со значением true и что она полностью вычислена с этим параметром. Если в этой ячейке нет ссылки на формулу, будет возвращено null. Для получения более подробной информации и примера см. [`GetDependentsInCalculation`](../../cell/getdependentsincalculation/).

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsMethodGetDependentsInCalculationWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создайте новую рабочую книгу и вычислите формулы
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Настройте зависимости формул:
            // C1 = 10 (исходное значение)
            // B1 = C1*2
            // A1 = B1+5
            cells["C1"].PutValue(10);
            cells["B1"].Formula = "C1*2";
            cells["A1"].Formula = "B1+5";

            // Вычислите формулы, чтобы установить зависимости
            workbook.CalculateFormula();

            try
            {
                // Получите зависимые элементы для ячейки C1 (строка 0, столбец 2) с рекурсивной проверкой
                IEnumerator dependents = cells.GetDependentsInCalculation(0, 2, true);

                Console.WriteLine("Dependents of cell C1:");
                while (dependents.MoveNext())
                {
                    if (dependents.Current is Cell dependentCell)
                    {
                        Console.WriteLine($"- {dependentCell.Name}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDependentsInCalculation: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("GetDependentsInCalculationDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


