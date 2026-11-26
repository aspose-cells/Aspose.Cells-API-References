---
title: "ProtectedRangeCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ProtectedRangeCollection. Добавляет элемент ProtectedRange в коллекцию"
type: docs
url: /ru/net/aspose.cells/protectedrangecollection/add/
---
## ProtectedRangeCollection.Add method

Добавляет элемент [`ProtectedRange`](../../protectedrange/) в коллекцию.

```csharp
public int Add(string name, int startRow, int startColumn, int endRow, int endColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | Заголовок диапазона. Используется как дескриптор, а не как определение именованного диапазона. |
| startRow | Int32 | Индекс начальной строки диапазона. |
| startColumn | Int32 | Индекс начального столбца диапазона. |
| endRow | Int32 | Индекс конечной строки диапазона. |
| endColumn | Int32 | Индекс конечного столбца диапазона. |

### Возвращаемое значение

Индекс объекта.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeCollectionMethodAddWithStringInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ProtectedRangeCollection pranges = workbook.Worksheets[0].AllowEditRanges;
            
            // Добавьте защищённый диапазон с именем и координатами
            int index = pranges.Add("Range1", 0, 0, 10, 10);
            
            // Получите доступ к добавленному диапазону
            ProtectedRange range = pranges[index];
            
            // Установить дескриптор безопасности
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            range.SecurityDescriptor = securityDescriptor;
            
            // Сохранить и проверить
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


