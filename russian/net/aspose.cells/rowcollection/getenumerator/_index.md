---
title: "RowCollection.GetEnumerator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод RowCollection. Возвращает перечислитель, который перебирает строки в этой коллекции"
type: docs
url: /ru/net/aspose.cells/rowcollection/getenumerator/
---
## GetEnumerator() {#getenumerator}

Возвращает перечислитель, который перебирает строки в этой коллекции

```csharp
public IEnumerator GetEnumerator()
```

### Возвращаемое значение

Перечислитель строк, который будет проходить по всем существующим строкам в этой коллекции.

### Примеры

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить высоту строк для демонстрации
            worksheet.Cells.SetRowHeight(0, 15);
            worksheet.Cells.SetRowHeight(1, 20);
            worksheet.Cells.SetRowHeight(2, 25);

            IEnumerator enumerator = worksheet.Cells.Rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine($"Row index: {row.Index}, Height: {row.Height}");
            }
        }
    }
}
```

### См. также

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

Возвращает перечислитель, который перебирает строки в этой коллекции

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| обратный | Boolean | нужно ли перечислять строки в обратном порядке |
| синхронный | Boolean | нужно ли возвращаемому перечислителю проверять изменение коллекции строк и оставаться синхронизированным с ней. |

### Возвращаемое значение

Перечислитель строк, который будет проходить по всем существующим строкам в этой коллекции.

### Примечания

Если коллекция строк будет изменена (операциями, которые могут привести к созданию новой Row или удалению существующей Row) во время обхода с помощью перечислителя, следует использовать синхронизированный перечислитель вместо обычного, чтобы обход мог продолжаться с позиции, следующей сразу после той, которую прошёл последний вызов MoveNext(). Однако, помимо преимущества в том, что ни один элемент не будет пропущен или пройден несколько раз, недостатком синхронизированного перечислителя является небольшое снижение производительности по сравнению с обычным перечислителем.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые примерные данные в строки
            for (int i = 0; i < 5; i++)
            {
                Row row = worksheet.Cells.Rows[i];
                row[0].PutValue($"Row {i + 1}");
            }
            
            try
            {
                // Получить RowCollection
                RowCollection rows = worksheet.Cells.Rows;
                
                // Вызовите GetEnumerator с параметрами (reversed: true, sync: false)
                IEnumerator enumerator = rows.GetEnumerator(true, false);
                
                Console.WriteLine("Iterating rows in reverse order:");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
                
                // Вызовите GetEnumerator с параметрами (reversed: false, sync: true)
                enumerator = rows.GetEnumerator(false, true);
                
                Console.WriteLine("\nIterating rows in normal order (synchronized):");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("RowCollectionGetEnumeratorDemo.xlsx");
        }
    }
}
```

### См. также

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


