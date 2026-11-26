---
title: "Worksheet.CalculateArrayFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Вычисляет формулу как массивную формулу"
type: docs
url: /ru/net/aspose.cells/worksheet/calculatearrayformula/
---
## CalculateArrayFormula(string, CalculationOptions) {#calculatearrayformula}

Вычисляет формулу как массивную формулу.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Формула для вычисления. |
| opts | CalculationOptions | Параметры вычисления формулы |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните некоторыми образцовыми данными
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // Определить массивную формулу
            string arrayFormula = "=SUM(A1:B3)";
            
            // Вычислить массивную формулу с параметрами расчёта
            object[][] result = worksheet.CalculateArrayFormula(arrayFormula, new CalculationOptions());
            
            // Вывести результат.
            Console.WriteLine("Result of array formula calculation: " + result[0][0]);
        }
    }
}
```

### См. также

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateArrayFormula(string, CalculationOptions, int, int) {#calculatearrayformula_1}

Вычисляет формулу как массивную формулу.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts, int maxRowCount, 
    int maxColumnCount)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Формула для вычисления. |
| opts | CalculationOptions | Параметры вычисления формулы |
| maxRowCount | Int32 | максимальное количество строк результирующих данных. Если оно неположительно или превышает фактическое количество строк, будет использовано фактическое количество строк. |
| maxColumnCount | Int32 | максимальное количество столбцов результирующих данных. Если оно неположительно или превышает фактическое количество столбцов, будет использовано фактическое количество столбцов. |

### Возвращаемое значение

Результат вычисленной формулы.

### Примечания

Формула будет рассматриваться как динамическая массивная формула для вычисления размеров и результата. Указанное пользователем максимальное измерение используется в случаях, когда вычисленный результат представляет большой набор данных (например, результат может соответствовать целой строке или столбцу), но пользователь не нуждается в таком большом массиве в соответствии с бизнес‑требованиями или соображениями производительности.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsInt32IDemo
    {
        public static void Run()
        {
            // Создайте книгу и откройте первый лист
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Пример 1: Простой расчёт массивной формулы
            string formula = "=ISBLANK(IF(TRUE,B2:B5))";
            CalculationOptions options = new CalculationOptions();
            object[][] result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of ISBLANK(IF(TRUE,B2:B5)): " + result[0][0]);

            // Пример 2: Массивная формула с динамическим диапазоном
            formula = "=LEN(IF({1;2;3;4},B2:B5))";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of LEN(IF({1;2;3;4},B2:B5)): " + result[0][0]);

            // Пример 3: Массивная формула с функцией MATCH
            // Создайте некоторые тестовые данные
            sheet.Cells["B2"].PutValue(5);
            sheet.Cells["B3"].PutValue(10);
            sheet.Cells["C2"].PutValue(1);
            sheet.Cells["C3"].PutValue(2);
            sheet.Cells["D2"].PutValue(0);
            sheet.Cells["D3"].PutValue(0);

            formula = "=MATCH(1,IF(B2:B5=5,C2:C5,D2:D5),0)";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of MATCH formula: " + result[0][0]);
        }
    }
}
```

### См. также

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) {#calculatearrayformula_2}

Вычисляет формулу как массивную формулу.

```csharp
public object[][] CalculateArrayFormula(string formula, FormulaParseOptions pOpts, 
    CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, 
    int maxColumnCount, CalculationData calculationData)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Формула для вычисления. |
| pOpts | FormulaParseOptions | Параметры разбора формулы |
| cOpts | CalculationOptions | Параметры вычисления формулы |
| baseCellRow | Int32 | Индекс строки базовой ячейки. |
| baseCellColumn | Int32 | Индекс столбца базовой ячейки. |
| maxRowCount | Int32 | Максимальное количество строк результирующих данных. Если оно неположительно или превышает фактическое количество строк, будет использовано фактическое количество строк. |
| maxColumnCount | Int32 | Максимальное количество столбцов результирующих данных. Если оно неположительно или превышает фактическое количество строк, будет использовано фактическое количество столбцов. |
| calculationData | CalculationData | Данные расчёта. Они используются в ситуации, когда пользователю необходимо вычислить некоторые статические формулы при реализации пользовательского движка расчётов. Для такой ситуации пользователь должен указать их с помощью данных расчёта, предоставленных для [`Calculate`](../../abstractcalculationengine/calculate/). |

### Возвращаемое значение

Результат вычисленной формулы.

### Примечания

Формула будет рассматриваться как динамическая массивная формула для вычисления размеров и результата. Указанное пользователем максимальное измерение используется в случаях, когда вычисленный результат представляет большой набор данных (например, результат может соответствовать целой строке или столбцу), но пользователь не нуждается в таком большом массиве в соответствии с бизнес‑требованиями или соображениями производительности.

### См. также

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


