---
title: "Cell.SetArrayFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Устанавливает массивную формулу в диапазон ячеек"
type: docs
url: /ru/net/aspose.cells/cell/setarrayformula/
---
## SetArrayFormula(string, int, int, bool, bool) {#setarrayformula_3}

Устанавливает массивную формулу для диапазона ячеек.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayFormula | String | Массивная формула. |
| rowNumber | Int32 | Количество строк для заполнения результата массивной формулы. |
| columnNumber | Int32 | Количество столбцов для заполнения результата массивной формулы. |
| isR1C1 | Boolean | является ли формула формулой R1C1 |
| isLocal | Boolean | является ли формула локализованной |

### Примечания

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо этого, пожалуйста, используйте Cell.SetArrayFormula(string,int,int,FormulaParseOptions). Это свойство будет удалено через 12 месяцев, начиная с декабря 2019 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetArrayFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;

            try
            {
                // Получить целевую ячейку, в которой мы хотим установить массивную формулу
                Cell targetCell = worksheet.Cells["B1"];

                // Установить массивную формулу, умножающую значения в A1:A3 на 2
                // Параметры: (formula, rowNumber=3, columnNumber=1, isR1C1=false, isLocal=false)
                targetCell.SetArrayFormula("=A1:A3*2", 3, 1, false, false);

                // Вычислите рабочую книгу, чтобы увидеть результаты
                workbook.CalculateFormula();

                // Отобразите результаты
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B2 value: {worksheet.Cells["B2"].Value}");
                Console.WriteLine($"B3 value: {worksheet.Cells["B3"].Value}");

                // Сохраните книгу
                workbook.Save("SetArrayFormulaDemo.xlsx");
                Console.WriteLine("Array formula set successfully and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting array formula: {ex.Message}");
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

## SetArrayFormula(string, int, int) {#setarrayformula}

Устанавливает массивную формулу (устаревшую массивную формулу, вводимую с помощью CTRL+SHIFT+ENTER в MS Excel) для диапазона ячеек.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayFormula | String | Массивная формула. |
| rowNumber | Int32 | Количество строк для заполнения результата массивной формулы. |
| columnNumber | Int32 | Количество столбцов для заполнения результата массивной формулы. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            Cell cell = cells["A1"];
            cell.SetArrayFormula("=FREQUENCY({\"79\",\"85\",\"78\",\"85\",\"50\",\"81\",\"95\",\"88\",\"97\"},{70,79,89})", 4, 1);

            workbook.CalculateFormula();

            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1} value: {cells[i, 0].IntValue}");
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

## SetArrayFormula(string, int, int, FormulaParseOptions) {#setarrayformula_1}

Устанавливает массивную формулу для диапазона ячеек.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayFormula | String | Массивная формула. |
| rowNumber | Int32 | Количество строк для заполнения результата массивной формулы. |
| columnNumber | Int32 | Количество столбцов для заполнения результата массивной формулы. |
| опции | FormulaParseOptions | Параметры разбора формулы. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Поместите примерные данные в ячейки C1:E1
            cells["C1"].PutValue(10);
            cells["D1"].PutValue(20);
            cells["E1"].PutValue(30);

            // Установите массивную формулу в ячейку A1, которая развернётся на 2 строки и 3 столбца
            cells["A1"].SetArrayFormula("=TRANSPOSE(C1:E1)", 2, 1, new FormulaParseOptions());

            // Вычислить формулы
            workbook.CalculateFormula();

            // Выведите результаты
            Console.WriteLine("Array formula results:");
            for (int row = 0; row < 2; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = cells[row, col];
                    Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                }
            }
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

## SetArrayFormula(string, int, int, FormulaParseOptions, object[][]) {#setarrayformula_2}

Устанавливает массивную формулу для диапазона ячеек.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayFormula | String | Массивная формула. |
| rowNumber | Int32 | Количество строк для заполнения результата массивной формулы. |
| columnNumber | Int32 | Количество столбцов для заполнения результата массивной формулы. |
| опции | FormulaParseOptions | Параметры разбора формулы. |
| значения | Object[][] | значения для этих ячеек с заданной массивной формулой |

### См. также

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


