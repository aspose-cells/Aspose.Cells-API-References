---
title: "WorksheetCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод WorksheetCollection. Удаляет элемент с указанным именем"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

Удаляет элемент по указанному имени.

```csharp
public void RemoveAt(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Имя удаляемого элемента. |

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Добавить несколько листов
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");
            
            // Добавить именованный диапазон (фиксированный)
            int nameIndex = wb.Worksheets.Names.Add("testname");
            wb.Worksheets.Names[nameIndex].RefersTo = "=[Book1.xlsx]Sheet1!$A1";
            
            // Продемонстрировать RemoveAt со строковым параметром
            Console.WriteLine($"Before removal - Worksheet count: {wb.Worksheets.Count}");
            wb.Worksheets.RemoveAt("Sheet1");
            Console.WriteLine($"After removal - Worksheet count: {wb.Worksheets.Count}");
            
            // Сохраните книгу
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
            }
        }
    }
}
```

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int) {#removeat}

Удаляет элемент по указанному индексу.

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс удаляемого элемента. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Добавить несколько листов
            wb.Worksheets.Add("Sheet1");
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");

            // Отобразить исходное количество листов
            Console.WriteLine($"Original worksheet count: {wb.Worksheets.Count}");

            // Удалить лист по индексу 1 (второй лист)
            wb.Worksheets.RemoveAt(1);

            // Отобразить обновлённое количество листов
            Console.WriteLine($"After removal, worksheet count: {wb.Worksheets.Count}");

            // Сохраните книгу
            wb.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


