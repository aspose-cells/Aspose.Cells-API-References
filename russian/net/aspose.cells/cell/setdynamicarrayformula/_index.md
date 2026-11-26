---
title: "Cell.SetDynamicArrayFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Устанавливает формулу динамического массива и, если возможно, позволяет формуле распространяться на соседние ячейки"
type: docs
url: /ru/net/aspose.cells/cell/setdynamicarrayformula/
---
## SetDynamicArrayFormula(string, FormulaParseOptions, bool) {#setdynamicarrayformula}

Устанавливает динамическую массивную формулу и, если возможно, позволяет ей вытекать в соседние ячейки.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    bool calculateValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayFormula | String | выражение формулы |
| опции | FormulaParseOptions | опции для разбора формулы. Параметр "Parse" будет игнорироваться, и формула всегда будет разбираться сразу |
| calculateValue | Boolean | нужно ли вычислять эту формулу динамического массива для ячеек в разливном диапазоне. |

### Возвращаемое значение

диапазон, в который формула должна разливаться.

### Примечания

возвращаемый диапазон может отличаться от фактического, в который эта формула динамического массива разливается. Если в диапазоне есть непустые ячейки, формула будет установлена только для текущей ячейки и помечена как "#SPILL!". Но в таком случае мы всё равно возвращаем весь диапазон, в который должна разливаться эта формула.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsBooleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Установить формулу динамического массива в ячейку A1
            Cell cell1 = cells["A1"];
            cell1.SetDynamicArrayFormula("=SEQUENCE(B2)", new FormulaParseOptions(), true);

            // Установить значение в B2, которое повлияет на формулу SEQUENCE
            cells["B2"].PutValue(3);

            // Вычислить формулы и обновить динамические массивы
            wb.CalculateFormula();
            wb.RefreshDynamicArrayFormulas(false);

            // Вывести результаты из разливного диапазона
            Console.WriteLine("Dynamic array results:");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine(cells[0, i].Value);
            }
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool) {#setdynamicarrayformula_1}

Устанавливает динамическую массивную формулу и, если возможно, позволяет ей вытекать в соседние ячейки.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayFormula | String | выражение формулы |
| опции | FormulaParseOptions | опции для разбора формулы. Параметр "Parse" будет игнорироваться, и формула всегда будет разбираться сразу |
| значения | Object[][] | значения (вычисленные результаты) для ячеек с заданной формулой динамического массива |
| calculateRange | Boolean | Нужно ли вычислять разливной диапазон для этой формулы динамического массива. Если параметр "values" не равен null и этот флаг установлен в false, то высота разливного диапазона будет values.Length, а ширина — values[0].Length. |
| calculateValue | Boolean | нужно ли вычислять эту формулу динамического массива для ячеек в разливном диапазоне, когда "values" равно null или соответствующий элемент в "values" для одной ячейки равен null. |

### Возвращаемое значение

диапазон, в который формула должна разливаться.

### Примечания

возвращаемый диапазон может отличаться от фактического, в который эта формула динамического массива разливается. Если в диапазоне есть непустые ячейки, формула будет установлена только для текущей ячейки и помечена как "#SPILL!". Но в таком случае мы всё равно возвращаем весь диапазон, в который должна разливаться эта формула.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue(10);
            cell = cells["A2"];
            cell.PutValue(20);
            cell = cells["B1"];
            cell.PutValue(60);
            cell = cells["B2"];
            cell.PutValue(80);

            // Получить ячейку C1, где будет установлена формула динамического массива
            cell = worksheet.Cells["C1"];

            // Определить формулу динамического массива
            string formula = "=A1:B2 * 2";
            
            // Создать параметры разбора формулы
            FormulaParseOptions options = new FormulaParseOptions
            {
                Parse = true // Enable formula parsing
            };

            // Подготовить значения для заполнения ячеек с результатами формулы
            object[][] values = new object[2][];
            values[0] = new object[] { 2, 4 };
            values[1] = new object[] { 6, 8 };

            try
            {
                // Установить формулу динамического массива с предварительно вычисленными значениями
                CellArea result = cell.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange: false,  // Use values array dimensions for spill range
                    calculateValue: false  // Use provided values instead of calculating
                );

                Console.WriteLine($"Dynamic array formula set. Affected range: Rows {result.StartRow}-{result.EndRow}, Columns {result.StartColumn}-{result.EndColumn}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula: {ex.Message}");
            }

            // Сохранить книгу с изменениями
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) {#setdynamicarrayformula_2}

Устанавливает динамическую массивную формулу и, если возможно, позволяет ей вытекать в соседние ячейки.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue, CalculationOptions copts)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayFormula | String | выражение формулы |
| опции | FormulaParseOptions | опции для разбора формулы. Параметр "Parse" будет игнорироваться, и формула всегда будет разбираться сразу |
| значения | Object[][] | значения (вычисленные результаты) для ячеек с заданной формулой динамического массива |
| calculateRange | Boolean | Нужно ли вычислять разливной диапазон для этой формулы динамического массива. Если параметр "values" не равен null и этот флаг установлен в false, то высота разливного диапазона будет values.Length, а ширина — values[0].Length. |
| calculateValue | Boolean | нужно ли вычислять эту формулу динамического массива для ячеек в разливном диапазоне, когда "values" равно null или соответствующий элемент в "values" для одной ячейки равен null. |
| copts | CalculationOptions | Опции для вычисления формулы. Обычно, с учётом производительности, свойство [`Recursive`](../../calculationoptions/recursive/) должно быть false. |

### Возвращаемое значение

диапазон, в который формула должна разливаться.

### Примечания

возвращаемый диапазон может отличаться от фактического, в который эта формула динамического массива разливается. Если в диапазоне есть непустые ячейки, формула будет установлена только для текущей ячейки и помечена как "#SPILL!". Но в таком случае мы всё равно возвращаем весь диапазон, в который должна разливаться эта формула.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить образцы данных в ячейках A2:B5
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(60);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B3"].PutValue(55);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["B5"].PutValue(70);

            // Получить целевую ячейку D1
            Cell cellD1 = worksheet.Cells["D1"];

            try
            {
                // Подготовить параметры для SetDynamicArrayFormula
                string formula = "=FILTER(A2:A5, B2:B5>50)";
                FormulaParseOptions options = new FormulaParseOptions { Parse = true };
                object[][] values = new object[2][] { new object[] { 10 }, new object[] { 40 } };
                bool calculateRange = true;
                bool calculateValue = true;
                CalculationOptions calcOptions = new CalculationOptions { Recursive = true };

                // Вызовите SetDynamicArrayFormula с конкретными параметрами
                CellArea spillRange = cellD1.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange,
                    calculateValue,
                    calcOptions
                );

                Console.WriteLine($"Dynamic array formula set successfully. Spill range: {spillRange}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


