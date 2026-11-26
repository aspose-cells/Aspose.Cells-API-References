---
title: "Cell.SetFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Установить формулу и вычисленный результат формулы"
type: docs
url: /ru/net/aspose.cells/cell/setformula/
---
## SetFormula(string, object) {#setformula_3}

Устанавливает формулу и значение (рассчитанный результат) формулы.

```csharp
public void SetFormula(string formula, object value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Формула. |
| значение | Object | Значение (вычисленный результат) формулы. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringObjectDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить формулу со строковыми и объектными параметрами
            cells["A1"].SetFormula("=SUM(1,2)", 4); // Will display 4 until calculation
            cells["A2"].SetFormula("=AVERAGE(5,10)", 7.5); // Will display 7.5 until calculation

            // Отобразить значения до вычисления
            Console.WriteLine("Before Calculation:");
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("A2: " + cells["A2"].StringValue);

            // Вычислить формулы
            workbook.CalculateFormula();

            // Отобразить значения после вычисления
            Console.WriteLine("\nAfter Calculation:");
            Console.WriteLine("A1: " + cells["A1"].IntValue); // Should show 3
            Console.WriteLine("A2: " + cells["A2"].DoubleValue); // Should show 7.5
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions) {#setformula}

Устанавливает формулу и значение (рассчитанный результат) формулы.

```csharp
public void SetFormula(string formula, FormulaParseOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Формула. |
| опции | FormulaParseOptions | Параметры разбора формулы. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить конкретную ячейку (в данном случае B2)
            Cell cell = worksheet.Cells["B2"];
            
            // Установить некоторые начальные значения для демонстрации
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            
            // Пример 1: Установить простую формулу с параметрами разбора по умолчанию
            cell.SetFormula("=SUM(A1:A2)", new FormulaParseOptions());
            Console.WriteLine("Formula with default options: " + cell.Formula);
            
            // Пример 2: Установить формулу в стиле R1C1 с использованием FormulaParseOptions
            FormulaParseOptions options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            
            cell.SetFormula("=SUM(R[-1]C[-1]:R[0]C[-1])", options);
            Console.WriteLine("Formula with R1C1 style: " + cell.Formula);
            
            // Пример 3: Установить формулу с параметрами разбора, сохраняющими формат R1C1
            options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            cell.SetFormula("=R1C1+R2C2", options);
            Console.WriteLine("Formula preserved as R1C1: " + cell.Formula);
            
            // Вычислите книгу, чтобы увидеть результаты
            workbook.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.Value);
        }
    }
}
```

### См. также

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, bool, bool, object) {#setformula_2}

Устанавливает формулу и значение формулы.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetFormula(string formula, bool isR1C1, bool isLocal, object value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Формула. |
| isR1C1 | Boolean | Является ли формула формулой R1C1. |
| isLocal | Boolean | Является ли формула локализованной. |
| значение | Object | Значение формулы. |

### Примечания

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него, пожалуйста, используйте Cell.SetFormula(string,FormulaParseOptions,object). Это свойство будет удалено через 12 месяцев, начиная с декабря 2019 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetFormulaWithStringBooleanBooleanObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);

            // Получите целевую ячейку, в которой мы установим формулу
            Cell cell = worksheet.Cells["C1"];

            try
            {
                // Установите формулу со всеми параметрами
                // Параметры: строка формулы, isR1C1, isLocal, значение
                cell.SetFormula("=SUM(A1:B2)", false, false, null);

                // Вычислить формулу
                workbook.CalculateFormula();

                // Отобразить результат
                Console.WriteLine($"Formula set successfully. Result: {cell.Value}");

                // Сохраните книгу
                workbook.Save("SetFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting formula: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions, object) {#setformula_1}

Устанавливает формулу и значение (рассчитанный результат) формулы.

```csharp
public void SetFormula(string formula, FormulaParseOptions options, object value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| формула | String | Формула. |
| опции | FormulaParseOptions | Параметры разбора формулы. |
| значение | Object | Значение (вычисленный результат) формулы. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Установите начальную формулу со ссылкой на надстройку
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Initial formula: " + sheet.Cells[0, 0].Formula);

            // Используйте SetFormula для переопределения без проверки надстройки
            sheet.Cells[0, 0].SetFormula("=dsfun(B1)", new FormulaParseOptions() { CheckAddIn = false }, null);
            Console.WriteLine("After SetFormula: " + sheet.Cells[0, 0].Formula);

            // Сбросить к формуле надстройки
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Reset to add-in formula: " + sheet.Cells[0, 0].Formula);

            // Создайте новую книгу и скопируйте лист
            Workbook wb2 = new Workbook();
            wb2.Worksheets[0].Cells[0, 0].Formula = "'externalDS.xlam'!dsfunnew(C1)";
            wb2.Worksheets[0].Copy(sheet);
            Console.WriteLine("After copy: " + wb2.Worksheets[0].Cells[0, 0].Formula);
        }
    }
}
```

### См. также

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


