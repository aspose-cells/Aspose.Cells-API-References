---
title: "Cells.ImportArray"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells."
type: docs
url: /ru/net/aspose.cells/cells/importarray/
---
## ImportArray(string[], int, int) {#importarray_4}

```csharp
public void ImportArray(string[] stringArray, int firstRow, int firstColumn)
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(string[], int, int, bool) {#importarray_5}

Импортирует массив string в рабочий лист.

```csharp
public void ImportArray(string[] stringArray, int firstRow, int firstColumn, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stringArray | String[] | Массив String. |
| firstRow | Int32 | Номер строки первой ячейки для импорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для импорта. |
| isVertical | Boolean | Указывает импортировать данные вертикально или горизонтально. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithStringInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовить данные массива строк
            string[] fruitArray = new string[] { "Apple", "Banana", "Cherry", "Date", "Elderberry" };

            try
            {
                // Вызвать ImportArray с параметрами: (String[], Int32, Int32, Boolean)
                // Начать импортировать с строки 2 (3‑я строка), столбца 1 (столбец B), вертикально
                worksheet.Cells.ImportArray(fruitArray, 2, 1, true);

                Console.WriteLine("Imported string array vertically starting from cell B3:");
                foreach (string fruit in fruitArray)
                {
                    Console.WriteLine(fruit);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("CellsMethodImportArrayWithStringInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(int[], int, int) {#importarray_2}

```csharp
public void ImportArray(int[] intArray, int firstRow, int firstColumn)
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(int[], int, int, bool) {#importarray_3}

Импортирует массив integer в рабочий лист.

```csharp
public void ImportArray(int[] intArray, int firstRow, int firstColumn, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| intArray | Int32[] | Массив Integer. |
| firstRow | Int32 | Номер строки первой ячейки для импорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для импорта. |
| isVertical | Boolean | Указывает импортировать данные вертикально или горизонтально. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithInt32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Подготовить данные массива Int32
            int[] data = new int[] { 1, 2, 3, 4, 5 };

            try
            {
                // Вызвать ImportArray с параметрами: (Int32[], firstRow=2, firstColumn=1, isVertical=true)
                worksheet.Cells.ImportArray(data, 2, 1, true);

                Console.WriteLine("Imported array vertically starting from cell B3:");
                for (int i = 0; i < data.Length; i++)
                {
                    Console.WriteLine($"Cell B{3 + i}: {worksheet.Cells[2 + i, 1].Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }

            // Сохранить результат
            workbook.Save("CellsMethodImportArrayWithInt32Int32Int32BooleanDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(double[], int, int) {#importarray}

```csharp
public void ImportArray(double[] doubleArray, int firstRow, int firstColumn)
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportArray(double[], int, int, bool) {#importarray_1}

Импортирует массив double в рабочий лист.

```csharp
public void ImportArray(double[] doubleArray, int firstRow, int firstColumn, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| doubleArray | Double[] | Массив Double. |
| firstRow | Int32 | Номер строки первой ячейки для импорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для импорта. |
| isVertical | Boolean | Указывает импортировать данные вертикально или горизонтально. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportArrayWithDoubleInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Подготовить примерные данные массива double
            double[] dataArray = new double[] { 1.23, 4.56, 7.89, 10.11, 12.13 };
            const int targetRow = 2;    // 0-based row index (3rd row)
            const int targetColumn = 1; // 0-based column index (2nd column)
            const bool isVertical = true;

            try
            {
                // Получить коллекцию ячеек и вызвать ImportArray
                Cells cells = worksheet.Cells;
                cells.ImportArray(dataArray, targetRow, targetColumn, isVertical);
                
                Console.WriteLine($"Imported {dataArray.Length} double values starting at row {targetRow + 1}, column {targetColumn + 1}");
                Console.WriteLine($"Data orientation: {(isVertical ? "Vertical" : "Horizontal")}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("CellsImportArrayDoubleVerticalDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


