---
title: "Row.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Row. Проверяет, относится ли этот объект к той же строке, что и другой."
type: docs
url: /ru/net/aspose.cells/row/equals/
---
## Equals(object) {#equals_1}

Проверяет, относится ли этот объект к той же строке, что и другой.

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object | другой объект |

### Возвращаемое значение

true, если два объекта ссылаются на одну и ту же строку.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте две строки для сравнения.
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];
            
            // Установите некоторые свойства, чтобы сделать строки различными.
            row1.Height = 20;
            row2.Height = 25;
            
            try
            {
                // Вызовите метод Equals с параметром Object.
                bool result1 = row1.Equals((object)row2);
                Console.WriteLine($"Comparing row1 with row2: {result1}");
                
                // Сравните row1 с самим собой.
                bool result2 = row1.Equals((object)row1);
                Console.WriteLine($"Comparing row1 with itself: {result2}");
                
                // Сравнить с null
                bool result3 = row1.Equals((object)null);
                Console.WriteLine($"Comparing row1 with null: {result3}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            workbook.Save("RowMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### См. также

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Row) {#equals}

Проверяет, относится ли этот объект к той же строке, что и другой объект строки.

```csharp
public bool Equals(Row row)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Row | другой объект строки |

### Возвращаемое значение

истина, если два объекта строки ссылаются на одну и ту же строку.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithRowDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте две строки для сравнения.
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];

            // Установите некоторые свойства, чтобы сделать строки различными.
            row1.Height = 20;
            row2.Height = 25;
            row1.IsHidden = false;
            row2.IsHidden = true;

            try
            {
                // Вызовите метод Equals для сравнения строк
                bool areEqual = row1.Equals(row2);

                // Отобразить результат
                Console.WriteLine($"Are rows equal? {areEqual}");

                // Создайте другую строку с теми же свойствами, что и row1
                Row row3 = worksheet.Cells.Rows[2];
                row3.Height = row1.Height;
                row3.IsHidden = row1.IsHidden;

                // Сравните row1 с row3 (должны быть равны)
                bool areEqual2 = row1.Equals(row3);
                Console.WriteLine($"Are rows equal after matching properties? {areEqual2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("RowEqualsDemo.xlsx");
        }
    }
}
```

### См. также

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


