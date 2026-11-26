---
title: "WorksheetCollection.GetRangeByName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorksheetCollection. Получает объект Range по предопределённому имени"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/getrangebyname/
---
## GetRangeByName(string) {#getrangebyname}

Получает объект Range по предопределённому имени.

```csharp
public Range GetRangeByName(string rangeName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rangeName | String | Имя диапазона. |

### Возвращаемое значение

Объект Range.

Возвращает null, если именованный диапазон не существует.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetRangeByNameWithStringDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте некоторые данные в ячейки
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["B1"].PutValue("Banana");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            
            // Создать именованный диапазон
            worksheet.Cells.CreateRange("A1:B2").Name = "FruitData";
            
            // Получить именованный диапазон с помощью GetRangeByName
            Aspose.Cells.Range namedRange = workbook.Worksheets.GetRangeByName("FruitData");
            
            // Отобразить информацию о диапазоне, если найдено
            if (namedRange != null)
            {
                Console.WriteLine("Range found: " + namedRange.Address);
                Console.WriteLine("First cell value: " + namedRange[0, 0].StringValue);
            }
            else
            {
                Console.WriteLine("Range not found");
            }
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRangeByName(string, int, bool) {#getrangebyname_1}

Получает [`Range`](../../range/) по предопределённому имени или имени таблицы

```csharp
public Range GetRangeByName(string rangeName, int currentSheetIndex, bool includeTable)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rangeName | String | Имя диапазона или имя таблицы. |
| currentSheetIndex | Int32 | Индекс листа. -1 представляет глобальный. |
| includeTable | Boolean | Указывает, проверять ли все таблицы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetRangeByNameWithStringInt32BooleanDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создать именованный диапазон
            Aspose.Cells.Range namedRange = worksheet.Cells.CreateRange("A1", "C3");
            namedRange.Name = "TestRange";
            
            // Добавить некоторые данные в диапазон
            for (int i = 0; i < 3; i++)
            {
                for (int j = 0; j < 3; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            try
            {
                // Вызвать GetRangeByName с параметрами (String, Int32, Boolean)
                Aspose.Cells.Range retrievedRange = workbook.Worksheets.GetRangeByName("TestRange", 0, true);
                
                Console.WriteLine("Method executed successfully with parameters (String, Int32, Boolean)");
                Console.WriteLine($"Retrieved range address: {retrievedRange.Address}");
                Console.WriteLine($"Range contains {retrievedRange.RowCount} rows and {retrievedRange.ColumnCount} columns");
                
                // Отобразить значения диапазона
                Console.WriteLine("Range values:");
                foreach (Cell cell in retrievedRange)
                {
                    Console.WriteLine($"{cell.Name}: {cell.Value}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRangeByName method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("WorksheetCollectionMethodGetRangeByNameDemo.xlsx");
        }
    }
}
```

### См. также

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


