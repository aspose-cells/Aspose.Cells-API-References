---
title: "Name.GetRanges"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Name. Получает все диапазоны, на которые ссылается это имя"
type: docs
url: /ru/net/aspose.cells/name/getranges/
---
## GetRanges() {#getranges}

Получает все диапазоны, на которые ссылается это имя.

```csharp
public Range[] GetRanges()
```

### Возвращаемое значение

Все диапазоны.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangesDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            
            // Создать именованный диапазон
            int index = workbook.Worksheets.Names.Add("Fruits");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // Получить диапазоны с пересчетом
            Aspose.Cells.Range[] ranges1 = name.GetRanges();
            Console.WriteLine("Ranges with recalculation:");
            PrintRanges(ranges1);
            
            // Получить диапазоны без пересчета
            Aspose.Cells.Range[] ranges2 = name.GetRanges(false);
            Console.WriteLine("\nRanges without recalculation:");
            PrintRanges(ranges2);
        }
        
        private static void PrintRanges(Aspose.Cells.Range[] ranges)
        {
            if (ranges != null)
            {
                foreach (Aspose.Cells.Range range in ranges)
                {
                    Console.WriteLine($"Range: {range.Address}");
                }
            }
            else
            {
                Console.WriteLine("No ranges found");
            }
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRanges(bool) {#getranges_1}

Получает все диапазоны, на которые ссылается это имя.

```csharp
public Range[] GetRanges(bool recalculate)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| пересчитать | Boolean | нужно ли пересчитать его, если это имя уже было вычислено до этого вызова. |

### Возвращаемое значение

Все диапазоны.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameMethodGetRangesWithBooleanDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые образцы данных.
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            
            // Создать именованный диапазон
            int index = workbook.Worksheets.Names.Add("TestRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // Получить диапазоны без пересчета
            Aspose.Cells.Range[] ranges1 = namedRange.GetRanges(false);
            Console.WriteLine("Ranges count (no recalc): " + ranges1.Length);
            
            // Получить диапазоны с пересчетом
            Aspose.Cells.Range[] ranges2 = namedRange.GetRanges();
            Console.WriteLine("Ranges count (with recalc): " + ranges2.Length);
            
            // Изменить диапазон и продемонстрировать пересчет
            worksheet.Cells["A4"].PutValue(30);
            namedRange.RefersTo = "=Sheet1!$A$1:$A$4";
            
            // Получить диапазоны с пересчетом и без него после изменения
            Aspose.Cells.Range[] ranges3 = namedRange.GetRanges(false);
            Console.WriteLine("Ranges count after mod (no recalc): " + ranges3.Length);
            
            Aspose.Cells.Range[] ranges4 = namedRange.GetRanges();
            Console.WriteLine("Ranges count after mod (with recalc): " + ranges4.Length);
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


