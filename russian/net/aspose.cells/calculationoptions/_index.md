---
title: "Класс CalculationOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.CalculationOptions. Представляет параметры расчёта"
type: docs
url: /ru/net/aspose.cells/calculationoptions/
---
## CalculationOptions class

Представляет параметры вычисления.

```csharp
public class CalculationOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CalculationOptions](calculationoptions/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [CalcStackSize](../../aspose.cells/calculationoptions/calcstacksize/) { get; set; } | Размер стека для рекурсивного расчёта ячеек. Значение по умолчанию — 200. |
| [CalculationMonitor](../../aspose.cells/calculationoptions/calculationmonitor/) { get; set; } | Монитор для пользователя, позволяющий отслеживать прогресс вычисления формул. |
| [CharacterEncoding](../../aspose.cells/calculationoptions/characterencoding/) { get; set; } | Указывает кодировку, используемую для кодирования/декодирования символов при вычислении формул. Для функций, таких как CHAR, CODE, результат вычисления зависит от региональных настроек и кодовой страницы среды по умолчанию. С помощью этого свойства пользователь может задать правильную кодировку, используемую этими функциями, чтобы получить ожидаемый результат. |
| [CustomEngine](../../aspose.cells/calculationoptions/customengine/) { get; set; } | Пользовательский движок вычисления формул для расширения движка расчётов по умолчанию в Aspose.Cells. |
| [IgnoreError](../../aspose.cells/calculationoptions/ignoreerror/) { get; set; } | Указывает, следует ли игнорировать ошибки, возникшие при вычислении формул. Ошибка может быть вызвана неподдерживаемой функцией, внешними ссылками и т.д. Значение по умолчанию — true. |
| [LinkedDataSources](../../aspose.cells/calculationoptions/linkeddatasources/) { get; set; } | Указывает источники данных для внешних ссылок, используемых в формулах. |
| [PrecisionStrategy](../../aspose.cells/calculationoptions/precisionstrategy/) { get; set; } | Указывает стратегию обработки точности вычислений. |
| [Recursive](../../aspose.cells/calculationoptions/recursive/) { get; set; } | Указывает, следует ли вычислять зависимые ячейки рекурсивно при расчете одной ячейки, если она зависит от других ячеек. Значение по умолчанию — true. |
| [RefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/refreshdynamicarrayformula/) { get; set; } | Указывает, следует ли обновлять формулы динамических массивов перед вычислением формул. |
| [UserSpecifiedRefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/) { get; } | Указывает, указал ли пользователь явно поведение обновления формул динамических массивов перед вычислением указанных формул. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class CalculationOptionsDemo
    {
        public static void CalculationOptionsExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue(10.555);
            worksheet.Cells["A2"].PutValue(20.6666);
            worksheet.Cells["A3"].PutValue(30.7777);
            worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";

            // Создайте экземпляр CalculationOptions
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                CalcStackSize = 200,
                PrecisionStrategy = CalculationPrecisionStrategy.Round,
                CharacterEncoding = Encoding.UTF8
            };

            // При необходимости вы можете задать пользовательский движок вычислений или монитор
            // calcOptions.CustomEngine = new MyCustomEngine();
            // calcOptions.CalculationMonitor = new MyCalculationMonitor();

            // Вычислите формулы в рабочей книге с указанными параметрами
            workbook.CalculateFormula(calcOptions);

            // Сохраните книгу
            workbook.Save("CalculationOptionsExample.xlsx");
            workbook.Save("CalculationOptionsExample.pdf");

        }
    }

    // Пример пользовательского движка вычислений (при необходимости)
    public class MyCustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Пользовательская логика вычислений
            string funcName = data.FunctionName.ToUpper();
            if (funcName == "MYFUNC")
            {
                // Пример пользовательской логики функции
                int count = data.ParamCount;
                object result = null;
                for (int i = 0; i < count; i++)
                {
                    object paramValue = data.GetParamValue(i);
                    if (paramValue is ReferredArea)
                    {
                        ReferredArea ra = (ReferredArea)paramValue;
                        paramValue = ra.GetValue(0, 0);
                    }
                    // Обработайте параметр здесь
                    // result = ...;
                }
                data.CalculatedValue = result;
            }
        }
    }

    // Пример пользовательского монитора вычислений (при необходимости)
    public class MyCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // Логика перед вычислением
            Console.WriteLine($"Before calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // Логика после вычисления
            Console.WriteLine($"After calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override bool OnCircular(System.Collections.IEnumerator circularCellsData)
        {
            // Обработать циклические ссылки
            Console.WriteLine("Circular reference detected.");
            return true; // Continue calculation
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


