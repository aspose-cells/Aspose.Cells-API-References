---
title: "Workbook.RefreshDynamicArrayFormulas"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Обновляет динамические массивные формулы, spill в новый диапазон соседних ячеек в соответствии с текущими данными. Другие формулы в книге не будут вычисляться рекурсивно, даже если они использовались динамическими массивными формулами"
type: docs
url: /ru/net/aspose.cells/workbook/refreshdynamicarrayformulas/
---
## RefreshDynamicArrayFormulas(bool) {#refreshdynamicarrayformulas}

Обновляет формулы динамических массивов (размещение в новый диапазон соседних ячеек в соответствии с текущими данными). Другие формулы в книге не будут вычисляться рекурсивно, даже если они использовались формулами динамических массивов.

```csharp
public void RefreshDynamicArrayFormulas(bool calculate)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| вычислять | Boolean | Определяет, вычисляет ли и обновляет значения ячеек для этих динамических массивных формул |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet1 = wb.Worksheets[0];
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");

            // Установите начальные данные и динамические массивные формулы
            sheet1.Cells["A1"].PutValue("B1:B3");
            sheet1.Cells["A2"].SetDynamicArrayFormula("=INDIRECT(A1)", new FormulaParseOptions(), true);
            sheet2.Cells["B1"].SetDynamicArrayFormula("=TRANSPOSE(Sheet1!A2#)", new FormulaParseOptions(), true);

            Console.WriteLine("Before refresh:");
            PrintSpillStatus(sheet1, sheet2);

            // Измените диапазон и обновите формулы
            sheet1.Cells["A1"].PutValue("B1:B5");
            wb.RefreshDynamicArrayFormulas(true);

            Console.WriteLine("\nAfter refresh:");
            PrintSpillStatus(sheet1, sheet2);
        }

        private static void PrintSpillStatus(Worksheet sheet1, Worksheet sheet2)
        {
            Console.WriteLine("Sheet1 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet1.Cells.CheckCell(i, 0);
                Console.WriteLine($"Row {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }

            Console.WriteLine("\nSheet2 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet2.Cells.CheckCell(0, i);
                Console.WriteLine($"Column {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshDynamicArrayFormulas(bool, CalculationOptions) {#refreshdynamicarrayformulas_1}

Обновляет формулы динамических массивов (размещение в новый диапазон соседних ячеек в соответствии с текущими данными).

```csharp
public void RefreshDynamicArrayFormulas(bool calculate, CalculationOptions copts)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| вычислять | Boolean | Определяет, вычисляет ли и обновляет значения ячеек для этих динамических массивных формул |
| copts | CalculationOptions | Параметры вычисления формул |

### Примечания

В целях повышения производительности мы не обновляем автоматически все динамические массивные формулы, когда изменяется сама формула или данные, на которые она ссылается. Поэтому пользователю необходимо вызывать этот метод вручную после операций, которые могут влиять на динамические массивные формулы, таких как импорт/установка значений ячеек, вставка/удаление строк/столбцов/диапазонов и т.д. Для большинства формул с функциями вычисление диапазона spill также требует вычисления формулы, поэтому обычно предпочтительно использовать значение true для флага "calculate". Если формула проста, например ссылка на диапазон или массив (например "=C1:E5", "={1,2;3,4}", ...), простая функция над диапазоном или массивом (например "=ABS(C1:E5)", "=1+{1,2;3,4}", ...), и все формулы будут вычислены позже (например с помощью [`CalculateFormula`](../calculateformula/)), то использование значения false для флага "calculate" может избежать двойного вычисления и повысить производительность.

### Примеры

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanCalculationOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте пример динамической массивной формулы
            worksheet.Cells["A1"].Formula = "=SEQUENCE(5)";
            
            // Создать параметры расчёта
            CalculationOptions opts = new CalculationOptions();
            opts.CalcStackSize = 100;
            
            // Обновить динамические массивные формулы с параметрами вычисления
            workbook.RefreshDynamicArrayFormulas(true, opts);
            
            // Вычислить формулы книги
            workbook.CalculateFormula(opts);
            
            // Вывести результат из A1:A5
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].Value);
            }
        }
    }
}
```

### См. также

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


