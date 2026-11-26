---
title: "HyperlinkCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод HyperlinkCollection. Удалить гиперссылку по указанному индексу в этой коллекции"
type: docs
url: /ru/net/aspose.cells/hyperlinkcollection/removeat/
---
## HyperlinkCollection.RemoveAt method

Удалить гиперссылку по указанному индексу в этой коллекции.

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | Индекс элемента, начиная с нуля. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте гиперссылку в ячейку A1
            sheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Проверьте, существует ли гиперсылка перед удалением
            Console.WriteLine("Hyperlinks count before removal: " + sheet.Hyperlinks.Count);
            
            // Удалить гиперссылку с индексом 0
            sheet.Hyperlinks.RemoveAt(0);
            
            // Проверьте, что гиперссылка была удалена
            Console.WriteLine("Hyperlinks count after removal: " + sheet.Hyperlinks.Count);
        }
    }
}
```

### См. также

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


