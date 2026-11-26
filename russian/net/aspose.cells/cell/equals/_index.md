---
title: "Cell.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cell. Проверяет, ссылается ли этот объект на ту же ячейку, что и другой."
type: docs
url: /ru/net/aspose.cells/cell/equals/
---
## Equals(object) {#equals_1}

Проверяет, ссылается ли этот объект на ту же ячейку, что и другой.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object | другой объект |

### Возвращаемое значение

true, если два объекта ссылаются на одну и ту же ячейку.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Доступ к ячейкам из разных мест
            Cell cellA1 = worksheet.Cells["A1"];
            Cell anotherCellA1 = worksheet.Cells[0, 0]; // Same physical cell as A1
            Cell cellB1 = worksheet.Cells["B1"];

            // Установите одинаковые значения в разных ячейках
            cellA1.PutValue("Aspose.Cells");
            cellB1.PutValue("Aspose.Cells");

            try
            {
                // Сравните одинаковые физические ссылки на ячейки
                bool sameCellComparison = cellA1.Equals(anotherCellA1);
                Console.WriteLine($"Same cell comparison: {sameCellComparison}"); // True

                // Сравнить разные ячейки с одинаковым содержимым
                bool differentCellComparison = cellA1.Equals(cellB1);
                Console.WriteLine($"Different cell comparison: {differentCellComparison}"); // False

                // Сравнить ячейку с объектом, не являющимся ячейкой
                bool invalidTypeComparison = cellA1.Equals("Aspose.Cells");
                Console.WriteLine($"Invalid type comparison: {invalidTypeComparison}"); // False
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("CellMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Cell) {#equals}

Проверяет, ссылается ли этот объект на ту же ячейку, что и другой объект ячейки.

```csharp
public bool Equals(Cell cell)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| ячейка | Ячейка | другой объект ячейки |

### Возвращаемое значение

true, если два объекта ячейки ссылаются на одну и ту же ячейку.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithCellDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать ячейки в разных местах (A1 и B1)
            Cell cellA1 = worksheet.Cells[0, 0];
            Cell cellB1 = worksheet.Cells[0, 1];

            // Установить одинаковые значения в обеих ячейках
            cellA1.Value = "Aspose.Cells Comparison";
            cellB1.Value = "Aspose.Cells Comparison";

            try
            {
                // Сравнить cellA1 с cellB1 (разные места)
                bool equalsResult = cellA1.Equals(cellB1);
                Console.WriteLine($"Cell A1 equals Cell B1: {equalsResult}");

                // Сравнить cellA1 с самим собой (один и тот же экземпляр)
                equalsResult = cellA1.Equals(cellA1);
                Console.WriteLine($"Cell A1 equals itself: {equalsResult}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("CellMethodEqualsWithCellDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


