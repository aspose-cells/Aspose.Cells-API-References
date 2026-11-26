---
title: "Cell.SetTableFormula"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Создать двухпеременную таблицу данных для заданного диапазона, начиная с этой ячейки"
type: docs
url: /ru/net/aspose.cells/cell/settableformula/
---
## SetTableFormula(int, int, string, string, object[][]) {#settableformula_3}

Создать двухпараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string rowInputCell, 
    string columnInputCell, object[][] values)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowNumber | Int32 | Количество строк для заполнения формулы. |
| columnNumber | Int32 | Количество столбцов для заполнения формулы. |
| rowInputCell | String | ячейка ввода строки |
| columnInputCell | String | ячейка ввода столбца |
| значения | Object[][] | значения для ячеек в диапазоне формулы таблицы |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringStringObjectArrayDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);

            // Целевая ячейка, где будет установлена формула таблицы
            Cell targetCell = worksheet.Cells["C3"];

            // Подготовить параметры для SetTableFormula
            int rowNumber = 3;
            int columnNumber = 2;
            string rowInputCell = "A1";
            string columnInputCell = "A2";
            object[][] values = new object[][]
            {
                new object[] { 1, 2 },    // Row 1 data
                new object[] { 3, 4 },    // Row 2 data
                new object[] { 5, 6 }     // Row 3 data
            };

            try
            {
                // Установить формулу таблицы в целевой ячейке
                targetCell.SetTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values);

                // Вычислить формулы книги для обновления результатов
                workbook.CalculateFormula();

                Console.WriteLine("Table formula set successfully. Check D1:" + targetCell.StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, string, bool, object[][]) {#settableformula_2}

Создать однопараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string inputCell, bool isRowInput, 
    object[][] values)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowNumber | Int32 | Количество строк для заполнения формулы. |
| columnNumber | Int32 | Количество столбцов для заполнения формулы. |
| inputCell | String | вводная ячейка |
| isRowInput | Boolean | Указывает, является ли вводная ячейка ячейкой ввода строки (true) или ячейкой ввода столбца (false). |
| значения | Object[][] | значения для ячеек в диапазоне формулы таблицы |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32StringBooleanObjectDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = worksheet.Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(100000);
            cells[1, 3].PutValue(0.05);
            cells[1, 4].PutValue(2);
            cells[2, 1].PutValue(360);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);
            
            try
            {
                // Подготовить параметры для SetTableFormula
                int rowCount = 3;
                int colCount = 3;
                object[][] inputValues = new object[][] 
                {
                    new object[] { 0.05, 0.06, 0.07 },
                    new object[] { 1000, 2000, 3000 },
                    new object[] { 100, 200, 300 }
                };

                // Получить целевую ячейку для таблицы данных (C3)
                Cell tableCell = worksheet.Cells["C3"];
                // Вызвать SetTableFormula с вариациями процентной ставки
                tableCell.SetTableFormula(
                    rowNumber: rowCount,
                    columnNumber: colCount,
                    inputCell: "A1",
                    isRowInput: true,
                    values: inputValues
                );

                // Вычислить формулы для обновления результатов таблицы
                workbook.CalculateFormula();

                Console.WriteLine("Data table created successfully with varying interest rates");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating data table: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("SetTableFormulaDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, int, int, object[][]) {#settableformula_1}

Создать двухпараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, 
    int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, 
    object[][] values)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowNumber | Int32 | Количество строк для заполнения формулы. |
| columnNumber | Int32 | Количество столбцов для заполнения формулы. |
| rowIndexOfRowInputCell | Int32 | индекс строки ячейки ввода строки |
| columnIndexOfRowInputCell | Int32 | индекс столбца входной ячейки строки |
| rowIndexOfColumnInputCell | Int32 | индекс строки входной ячейки столбца |
| columnIndexOfColumnInputCell | Int32 | индекс столбца входной ячейки столбца |
| значения | Object[][] | значения для ячеек в диапазоне формулы таблицы |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(2);
            cells[1, 3].PutValue(3);
            cells[1, 4].PutValue(4);
            cells[2, 1].PutValue(2);
            cells[3, 1].PutValue(3);
            cells[4, 1].PutValue(4);
            
            Cell formulaCell = cells[2, 2];

            // Подготовьте входные значения для таблицы данных (процентные ставки и суммы кредитов)
            object[][] tableValues = new object[3][];
            tableValues[0] = new object[] { 0.05, 0.06, 0.07 };
            tableValues[1] = new object[] { 1000, 2000, 3000 };
            tableValues[2] = new object[] { 100, 200, 300 };

            try
            {
                // Установите формулу таблицы с размерами таблицы данных 3x3 и смещениями входной ячейки
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 3,
                    rowIndexOfRowInputCell: 0,  
                    columnIndexOfRowInputCell: 0,   
                    rowIndexOfColumnInputCell: 1,   
                    columnIndexOfColumnInputCell: 0, 
                    values: tableValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Data table formula set successfully. Check B2:D4 in output.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            workbook.Save("CellTableFormulaDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetTableFormula(int, int, int, int, bool, object[][]) {#settableformula}

Создать однопараметрическую таблицу данных для указанного диапазона, начиная с этой ячейки.

```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, 
    int columnIndexOfInputCell, bool isRowInput, object[][] values)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rowNumber | Int32 | Количество строк для заполнения формулы. |
| columnNumber | Int32 | Количество столбцов для заполнения формулы. |
| rowIndexOfInputCell | Int32 | индекс строки входной ячейки |
| columnIndexOfInputCell | Int32 | индекс столбца входной ячейки |
| isRowInput | Boolean | Указывает, является ли вводная ячейка ячейкой ввода строки (true) или ячейкой ввода столбца (false). |
| значения | Object[][] | значения для ячеек в диапазоне формулы таблицы |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetTableFormulaWithInt32Int32Int32Int32BooleanObjDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = workbook.Worksheets[0].Cells;
            cells[1, 1].Formula = "=A1+A2";

            cells[1, 2].PutValue(20);
            cells[1, 3].PutValue(30);            
            cells[2, 1].PutValue(20);
            cells[3, 1].PutValue(30);
            cells[4, 1].PutValue(40);

            // Создайте массив образцовых данных для параметров формулы таблицы
            object[][] inputValues = new object[][]
            {
                new object[] { 10, 20 },
                new object[] { 30, 40 },
                new object[] { 50, 60 }
            };

            // Получите целевую ячейку для применения формулы таблицы
            Cell formulaCell = worksheet.Cells[2, 2];

            try
            {
                // Установите формулу таблицы с: 
                // 3 строки, 2 столбца, входная ячейка в A1 (0,0), 
                // тип ввода строки и образцовые значения
                formulaCell.SetTableFormula(
                    rowNumber: 3,
                    columnNumber: 2,
                    rowIndexOfInputCell: 0,
                    columnIndexOfInputCell: 0,
                    isRowInput: true,
                    values: inputValues
                );

                workbook.CalculateFormula();
                Console.WriteLine("Table formula applied successfully. " + 
                    "Saved workbook with 3x2 table formula at C3.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting table formula: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("TableFormulaDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


