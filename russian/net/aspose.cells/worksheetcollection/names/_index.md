---
title: "WorksheetCollection.Names"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WorksheetCollection. Возвращает коллекцию всех объектов Name в таблице"
type: docs
url: /ru/net/aspose.cells/worksheetcollection/names/
---
## WorksheetCollection.Names property

Получает коллекцию всех объектов Name в таблице.

```csharp
public NameCollection Names { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyNamesDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист с особыми символами в имени
            Worksheet worksheet = workbook.Worksheets.Add("My.Test");
            
            // Доступ к коллекции Names
            NameCollection names = workbook.Worksheets.Names;
            
            // Добавьте новый именованный диапазон
            int index = names.Add("My.Test!TestName");
            Name namedRange = names[index];
            
            // Установите ссылку диапазона и продемонстрируйте использование
            namedRange.RefersTo = "=My.Test!$A$1:$B$2";
            
            // Выведите свойства именованного диапазона
            Console.WriteLine("Name: " + namedRange.Text);
            Console.WriteLine("FullText: " + namedRange.FullText);
            Console.WriteLine("RefersTo: " + namedRange.RefersTo);
        }
    }
}
```

### См. также

* class [NameCollection](../../namecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


