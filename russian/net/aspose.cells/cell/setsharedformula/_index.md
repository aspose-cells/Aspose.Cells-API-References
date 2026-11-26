---
title: "Cell.SetSharedFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Устанавливает формулу для диапазона ячеек"
type: docs
url: /ru/net/aspose.cells/cell/setsharedformula/
---
## SetSharedFormula(string, int, int, bool, bool) {#setsharedformula_3}

Устанавливает формулу для диапазона ячеек.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sharedFormula | String | Общая формула. |
| rowNumber | Int32 | Количество строк для заполнения формулы. |
| columnNumber | Int32 | Количество столбцов для заполнения формулы. |
| isR1C1 | Boolean | является ли формула формулой R1C1 |
| isLocal | Boolean | является ли формула локализованной |

### Примечания

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Вместо него используйте Cell.SetSharedFormula(string,int,int,FormulaParseOptions). Это свойство будет удалено через 12 месяцев, начиная с декабря 2019 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            // Заполнить примерными данными столбец A
            for (int row = 0; row < 5; row++)
            {
                cells[row, 0].Value = row + 1; // A1-A5: 1-5
            }

            // Получить целевую ячейку B1 для установки общей формулы
            Cell targetCell = cells[0, 1]; // B1

            try
            {
                // Установить общую формулу для вычисления квадрата значений в столбце A
                // Параметры: (formula, rowCount=5, columnCount=1, isR1C1=false, isLocal=false)
#pragma warning disable 0618 // Disable obsolete warning for demonstration
                targetCell.SetSharedFormula("=A1^2", 5, 1, false, false);
#pragma warning restore 0618

                // Проверить распространение формулы
                Console.WriteLine($"B1 formula: {targetCell.Formula}");
                Console.WriteLine($"B5 formula: {cells[4, 1].Formula}");

                // Вычислить рабочую книгу, чтобы обновить результаты формул
                workbook.CalculateFormula();

                Console.WriteLine($"A1 value: {cells["A1"].Value}");
                Console.WriteLine($"A5 value: {cells["A5"].Value}");
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B5 value: {cells[4, 1].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
                return;
            }

            // Сохранить изменённую книгу
            workbook.Save("SetSharedFormulaDemo.xlsx");
            Console.WriteLine("Spreadsheet saved successfully.");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetSharedFormula(string, int, int) {#setsharedformula}

Устанавливает общие формулы для диапазона ячеек.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sharedFormula | String | Общая формула. |
| rowNumber | Int32 | Количество строк для заполнения формулы. |
| columnNumber | Int32 | Количество столбцов для заполнения формулы. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetSharedFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Установить общую формулу в столбце B, начиная с B1 до B20
            cells["B1"].SetSharedFormula("=C1*2", 20, 1);

            // Установить некоторые значения в столбце C, чтобы продемонстрировать вычисление формулы
            for (int i = 0; i < 20; i++)
            {
                cells[i, 2].PutValue(i + 1); // Column C values (C1=1, C2=2...)
            }

            // Вычислить формулы
            workbook.CalculateFormula();

            // Вывести результаты для проверки
            for (int i = 0; i < 5; i++) // Display first 5 results
            {
                Console.WriteLine($"B{i+1} value: {cells[i, 1].Value}");
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

## SetSharedFormula(string, int, int, FormulaParseOptions) {#setsharedformula_1}

Устанавливает общие формулы для диапазона ячеек.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sharedFormula | String | Общая формула. |
| rowNumber | Int32 | Количество строк для заполнения формулы. |
| columnNumber | Int32 | Количество столбцов для заполнения формулы. |
| опции | FormulaParseOptions | Параметры разбора формулы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполнить примерными данными столбец A
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Получить целевую ячейку, где мы установим общую формулу
            Cell targetCell = worksheet.Cells["B1"];

            try
            {
                // Создать параметры разбора формулы со значениями по умолчанию
                FormulaParseOptions options = new FormulaParseOptions();

                // Установить общую формулу для 3 строк и 2 столбцов, начиная с B1
                targetCell.SetSharedFormula("=A1*2", 3, 2, options);

                Console.WriteLine("Shared formula set successfully for B1:C3 range");
                Console.WriteLine("B1 formula: " + worksheet.Cells["B1"].Formula);
                Console.WriteLine("C3 formula: " + worksheet.Cells["C3"].Formula);

                workbook.CalculateFormula();
                Console.WriteLine("B3 value: " + worksheet.Cells["B3"].Value);
                Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
                Console.WriteLine("C3 value: " + worksheet.Cells["C3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("SetSharedFormulaDemo.xlsx");
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

## SetSharedFormula(string, int, int, FormulaParseOptions, object[][]) {#setsharedformula_2}

Устанавливает общие формулы для диапазона ячеек.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| sharedFormula | String | Общая формула. |
| rowNumber | Int32 | Количество строк для заполнения формулы. |
| columnNumber | Int32 | Количество столбцов для заполнения формулы. |
| опции | FormulaParseOptions | Параметры разбора формулы. |
| значения | Object[][] | значения для этих ячеек с заданной общей формулой |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo1
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Установить примерное значение в ячейку A1
            worksheet.Cells["A1"].PutValue(5);

            // Получить целевую ячейку B2, где будет установлена общая формула
            Cell cell = worksheet.Cells["B2"];

            try
            {
                // Определить параметры общей формулы
                string formula = "=A1*2";
                int totalRows = 2;
                int totalColumns = 2;
                FormulaParseOptions parseOptions = new FormulaParseOptions();
                object[][] presetValues = new object[2][]
                {
                    new object[] { 10, 10 },
                    new object[] { 10, 10 }
                };

                // Установить общую формулу для диапазона 2x2, начиная с B2, с предустановленными значениями
                cell.SetSharedFormula(formula, totalRows, totalColumns, parseOptions, presetValues);

                Console.WriteLine("Shared formula set successfully. Cells B2:C3 contain values 10");
                workbook.CalculateFormula();
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "C3");
                IEnumerator iter = range.GetEnumerator();
                while(iter.MoveNext()) 
                {
                    Cell temp = (Cell)iter.Current;
                    Console.WriteLine(temp.Name + "  " + temp.Value);
                }

            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("SetSharedFormulaDemo.xlsx");
        }
    }
}
```

### См. также

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


