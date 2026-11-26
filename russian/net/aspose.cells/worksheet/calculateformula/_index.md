---
title: "Worksheet.CalculateFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Вычисляет формулу"
type: docs
url: /ru/net/aspose.cells/worksheet/calculateformula/
---
## CalculateFormula(string) {#calculateformula}

Вычисляет формулу.

```csharp
public object CalculateFormula(string formula)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Формула для вычисления. |

### Возвращаемое значение

Результат вычисленной формулы.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Worksheet sheet = wb.Worksheets[0];

            // Продемонстрировать базовое преобразование чисел
            string formula = "=NUMBERVALUE(\"1.234\")";
            Console.WriteLine("NUMBERVALUE(\"1.234\") = " + sheet.CalculateFormula(formula));

            // Продемонстрировать преобразование валют
            formula = "=NUMBERVALUE(\"$1,234.56\")";
            Console.WriteLine("NUMBERVALUE(\"$1,234.56\") = " + sheet.CalculateFormula(formula));

            // Продемонстрировать преобразование времени
            formula = "=NUMBERVALUE(\"0:25\")";
            Console.WriteLine("NUMBERVALUE(\"0:25\") = " + sheet.CalculateFormula(formula));

            // Продемонстрировать преобразование даты
            formula = "=NUMBERVALUE(\"07/26/2023\")";
            Console.WriteLine("NUMBERVALUE(\"07/26/2023\") = " + sheet.CalculateFormula(formula));

            // Продемонстрировать случай ошибки
            formula = "=NUMBERVALUE(\"invalid\")";
            Console.WriteLine("NUMBERVALUE(\"invalid\") = " + sheet.CalculateFormula(formula));
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(string, CalculationOptions) {#calculateformula_1}

Вычисляет выражение формулы напрямую.

```csharp
public object CalculateFormula(string formula, CalculationOptions opts)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Формула для вычисления. |
| opts | CalculationOptions | Параметры вычисления формулы |

### Возвращаемое значение

Вычисленный результат заданной формулы. Возвращаемый объект может быть одного из возможных типов [`Value`](../../cell/value/), или ReferredArea.

### Примечания

Формула будет вычислена так же, как если бы она была установлена в ячейку A1. И формула будет рассматриваться как обычная формула. Если вам необходимо вычислить формулу как массивную формулу и получить массив для вычисленного результата, пожалуйста, используйте [`CalculateArrayFormula`](../calculatearrayformula/) вместо этого.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните некоторыми образцовыми данными
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Создайте пользовательский движок вычислений
            CustomEngine customEngine = new CustomEngine();
            
            // Вычислить формулу с использованием пользовательского движка
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };
            
            object result = worksheet.CalculateFormula("=SUM(A1:A3)", options);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }

    public class CustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object value = data.GetParamValue(i);
                    if (value is double)
                    {
                        sum += (double)value;
                    }
                }
                data.CalculatedValue = sum;
            }
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

## CalculateFormula(string, FormulaParseOptions, CalculationOptions, int, int, CalculationData) {#calculateformula_2}

Вычисляет выражение формулы напрямую.

```csharp
public object CalculateFormula(string formula, FormulaParseOptions pOpts, CalculationOptions cOpts, 
    int baseCellRow, int baseCellColumn, CalculationData calculationData)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Формула для вычисления. |
| pOpts | FormulaParseOptions | Параметры разбора формулы. |
| cOpts | CalculationOptions | Параметры вычисления формулы. |
| baseCellRow | Int32 | Индекс строки базовой ячейки. |
| baseCellColumn | Int32 | Индекс столбца базовой ячейки. |
| calculationData | CalculationData | Данные расчёта. Они используются в ситуации, когда пользователю необходимо вычислить некоторые статические формулы при реализации пользовательского движка расчётов. Для такой ситуации пользователь должен указать их с помощью данных расчёта, предоставленных для [`Calculate`](../../abstractcalculationengine/calculate/). |

### Возвращаемое значение

Вычисленный результат заданной формулы. Возвращаемый объект может быть одного из возможных типов [`Value`](../../cell/value/), или ReferredArea.

### Примечания

Формула будет вычислена так же, как если бы она была установлена в указанную базовую ячейку. И формула будет рассматриваться как обычная формула. Если вам нужно, чтобы формула вычислялась как массивная формула и получить массив для вычисленного результата, пожалуйста, используйте [`CalculateArrayFormula`](../calculatearrayformula/) вместо этого.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringFormulaParseOptCalculati169472Demo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполнить примерными данными
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C1"].PutValue(2);
            worksheet.Cells["C2"].PutValue(4);

            // Определить параметры расчёта
            CalculationOptions calculationOptions = new CalculationOptions();
            
            // Определить параметры разбора формулы
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions();
            
            // Вычислить формулу со всеми параметрами
            object result = worksheet.CalculateFormula(
                "=SUM(B1:B2, C1:C2)",  // formula
                formulaParseOptions,   // parse options
                calculationOptions,    // calculation options
                0,                     // base cell row
                0,                     // base cell column
                null                   // calculation data
            );

            // Вывести результат.
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### См. также

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions, bool) {#calculateformula_3}

Вычисляет все формулы в этом листе.

```csharp
public void CalculateFormula(CalculationOptions options, bool recursive)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| опции | CalculationOptions | Параметры расчёта |
| recursive | Boolean | True означает, что если ячейки листа зависят от ячеек других листов, зависимые ячейки в других листах также будут вычислены. False означает, что все формулы на листе уже вычислены и значения верны. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithCalculationOptionsBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить примерные данные и формулы
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue("=SUM(A1:A3)");
            
            // Создать параметры расчёта
            CalculationOptions options = new CalculationOptions();
            options.Recursive = true;
            options.IgnoreError = false;
            
            // Вычислить формулу с параметрами и принудительно выполнить полное вычисление
            worksheet.CalculateFormula(options, true);
            
            // Вывести вычисленный результат
            Console.WriteLine("Calculated value: " + worksheet.Cells["B1"].StringValue);
        }
    }
}
```

### См. также

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


