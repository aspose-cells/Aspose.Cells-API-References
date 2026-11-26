---
title: "CellWatchCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellWatchCollection. Добавляет CellWatch с указанием строки и столбца"
type: docs
url: /ru/net/aspose.cells/cellwatchcollection/add/
---
## Add(int, int) {#add}

Добавляет [`CellWatch`](../../cellwatch/) с указанием строки и столбца.

```csharp
public int Add(int row, int column)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| строка | Int32 | Индекс строки. |
| column | Int32 | Индекс столбца. |

### Возвращаемое значение

Возвращает позицию этого элемента в коллекции.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить CellWatchCollection из рабочего листа.
            CellWatchCollection cellWatchCollection = worksheet.CellWatches;
            
            try
            {
                // Вызвать метод Add с индексами строки и столбца (Int32, Int32).
                int index = cellWatchCollection.Add(5, 3); // Adding cell at row 6, column D (0-based)
                
                Console.WriteLine($"CellWatch added at index: {index}");
                
                // Проверьте добавленный cell watch.
                CellWatch cellWatch = cellWatchCollection[index];
                Console.WriteLine($"Watching cell: {cellWatch.Row},{cellWatch.Column}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("CellWatchCollectionMethodAddWithInt32Int32Demo.xlsx");
        }
    }
}
```

### См. также

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Добавляет [`CellWatch`](../../cellwatch/) с именем ячейки.

```csharp
public int Add(string cellName)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cellName | String | Имя ячейки. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте несколько наблюдений за ячейками
            worksheet.CellWatches.Add("A1");
            worksheet.CellWatches.Add("B2");
            worksheet.CellWatches.Add("C3");
            
            // Отобразить количество cell watches.
            Console.WriteLine("Cell Watches Count: " + worksheet.CellWatches.Count);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [CellWatchCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


