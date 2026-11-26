---
title: "OleObjectCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод OleObjectCollection. Удаляет элемент по указанному индексу"
type: docs
url: /ru/net/aspose.cells.drawing/oleobjectcollection/removeat/
---
## OleObjectCollection.RemoveAt method

Удаляет элемент по указанному индексу.

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Указанный индекс. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте примерные OLE-объекты (3 объекта)
            for (int i = 0; i < 3; i++)
            {
                sheet.OleObjects.Add(i * 10, i * 10, 100, 100, new byte[0]);
            }

            Console.WriteLine("Before removal - OLE Objects count: " + sheet.OleObjects.Count);
            
            // Удаляйте OLE-объекты по одному с помощью RemoveAt(int index)
            for (int i = sheet.OleObjects.Count - 1; i >= 0; i--)
            {
                sheet.OleObjects.RemoveAt(i);
            }

            Console.WriteLine("After removal - OLE Objects count: " + sheet.OleObjects.Count);
        }
    }
}
```

### См. также

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


