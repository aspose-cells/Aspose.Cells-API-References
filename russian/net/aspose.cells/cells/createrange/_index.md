---
title: "Cells.CreateRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Создаёт объект Range из диапазона ячеек"
type: docs
url: /ru/net/aspose.cells/cells/createrange/
---
## CreateRange(string, string) {#createrange_3}

Создаёт объект [`Range`](../../range/) из диапазона ячеек.

```csharp
public Range CreateRange(string upperLeftCell, string lowerRightCell)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| upperLeftCell | String | Имя ячейки в левом верхнем углу. |
| lowerRightCell | String | Имя ячейки в правом нижнем углу. |

### Возвращаемое значение

Объект [`Range`](../../range/)

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Создать диапазон от A1 до A2
            Aspose.Cells.Range range = cells.CreateRange("A1", "A2");
            range.Name = "MyRange";
            
            // Установить значения в диапазоне
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            
            // Использовать диапазон в формуле
            cells["B1"].Formula = "=SUM(MyRange)";
            
            // Вычислить формулу
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of MyRange (A1:A2) is: " + cells["B1"].IntValue);
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, int, int) {#createrange_1}

Создаёт объект [`Range`](../../range/) из диапазона ячеек.

```csharp
public Range CreateRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstRow | Int32 | Первая строка этого диапазона |
| firstColumn | Int32 | Первый столбец этого диапазона |
| totalRows | Int32 | Количество строк |
| totalColumns | Int32 | Количество столбцов |

### Возвращаемое значение

Объект [`Range`](../../range/)

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать исходный диапазон (начиная со строки 2, столбца 2, с 3 строками и 4 столбцами)
            Aspose.Cells.Range rangeSrc = cells.CreateRange(2, 2, 3, 4);

            // Заполните исходный диапазон образцовыми данными
            for (int i = 0; i < rangeSrc.RowCount; i++)
            {
                for (int j = 0; j < rangeSrc.ColumnCount; j++)
                {
                    rangeSrc[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Создайте диапазон назначения (начиная с строки 8, столбца 0 с теми же размерами)
            Aspose.Cells.Range rangeDest = cells.CreateRange(8, 0, 3, 4);

            // Скопируйте значения из источника в назначение
            rangeDest.CopyValue(rangeSrc);

            // Сохраните книгу
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(string) {#createrange_2}

Создаёт объект [`Range`](../../range/) из адреса диапазона.

```csharp
public Range CreateRange(string address)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| address | String | Адрес диапазона. |

### Возвращаемое значение

Объект [`Range`](../../range/)

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте диапазон, используя строковый адрес
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Заполните данные в диапазоне
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // Создайте другой диапазон в новом листе
            workbook.Worksheets.Add();
            Worksheet worksheet2 = workbook.Worksheets[1];
            Aspose.Cells.Range range2 = worksheet2.Cells.CreateRange("A1:C3");

            // Скопируйте данные между диапазонами
            range2.Copy(range);

            // Сохраните книгу
            workbook.Save("CreateRangeWithStringDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, bool) {#createrange}

Создаёт объект [`Range`](../../range/) из строк ячеек или столбцов ячеек.

```csharp
public Range CreateRange(int firstIndex, int number, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| firstIndex | Int32 | Индекс первой строки или первого столбца, начиная с нуля. |
| число | Int32 | Общее количество строк или столбцов, начиная с единицы. |
| isVertical | Boolean | True — диапазон создан из столбцов ячеек. False — диапазон создан из строк ячеек. |

### Возвращаемое значение

Объект [`Range`](../../range/).

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создайте диапазон, начинающийся с ячейки A1 (0,0) с 5 строками и 3 столбцами
            Aspose.Cells.Range range = cells.CreateRange(0, 0, true);

            // Заполните диапазон некоторыми данными
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Row {i}, Col {j}");
                }
            }

            // Сохраните книгу
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


