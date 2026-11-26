---
title: "Row.GetEnumerator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Row. Получает перечислитель ячеек"
type: docs
url: /ru/net/aspose.cells/row/getenumerator/
---
## GetEnumerator() {#getenumerator}

Получает перечислитель ячеек

```csharp
public IEnumerator GetEnumerator()
```

### Возвращаемое значение

Перечислитель ячеек, который будет проходить все существующие ячейки в этой строке.

### Примеры

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Заполните некоторыми образцовыми данными
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            // Получить перечислитель для первой строки (строка заголовка)
            IEnumerator en = cells.Rows[0].GetEnumerator();
            while (en.MoveNext())
            {
                Cell cell = (Cell)en.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }
        }
    }
}
```

### См. также

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Получает перечислитель, который перебирает ячейки в этой строке.

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| обратный | Boolean | нужно ли перечислять ячейки в обратном порядке |
| синхронный | Boolean | нужно ли возвращаемому перечислителю проверять изменение ячеек в этой строке и поддерживать синхронизацию с ними. |

### Возвращаемое значение

Перечислитель ячеек, который будет проходить все существующие ячейки в этой строке.

### Примечания

Если строка будет изменена (операциями, которые могут привести к созданию новой ячейки или удалению существующей ячейки) во время обхода с помощью перечислителя, следует использовать синхронизированный перечислитель вместо обычного, чтобы обход мог продолжаться с позиции сразу после той, которая была пройдена последним вызовом MoveNext(). Однако, помимо преимущества, что ни один элемент не будет пропущен или пройден несколько раз, недостатком синхронизированного перечислителя является небольшое снижение производительности по сравнению с обычным перечислителем.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте некоторые данные в ячейки первой строки
            Row row = worksheet.Cells.Rows[0];
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            try
            {
                // Вызовите GetEnumerator с reversed=false и sync=true
                IEnumerator enumerator = row.GetEnumerator(false, true);
                
                Console.WriteLine("Cells in row 1:");
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }

                // Вызовите GetEnumerator с reversed=true и sync=false, чтобы продемонстрировать обратную итерацию
                Console.WriteLine("\nCells in row 1 (reversed order):");
                enumerator = row.GetEnumerator(true, false);
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("RowMethodGetEnumeratorWithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### См. также

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


