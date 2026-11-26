---
title: "NameCollection.RemoveAt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод NameCollection. Удаляет имя по указанному индексу"
type: docs
url: /ru/net/aspose.cells/namecollection/removeat/
---
## NameCollection.RemoveAt method

Удаляет имя по конкретному индексу.

```csharp
public void RemoveAt(int index)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| индекс | Int32 | индекс имени, которое нужно удалить. |

### Примечания

Пожалуйста, убедитесь, что имя не используется другими формулами перед вызовом метода. И если имя используется, лучше установить Name.RefersTo в null.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;
            NameCollection names = worksheets.Names;

            // Добавьте имена в коллекцию
            int firstIndex = names.Add("FirstRange");
            names[firstIndex].RefersTo = "=Sheet1!$A$1:$A$5";
            
            int secondIndex = names.Add("SecondRange");
            names[secondIndex].RefersTo = "=Sheet1!$B$1:$B$5";

            // Удалить имя по индексу
            names.RemoveAt(firstIndex);

            // Проверьте удаление, проверив количество
            Console.WriteLine($"Remaining names count: {names.Count}");

            workbook.Save("NameCollectionRemoveAtExample.xlsx");
        }
    }
}
```

### См. также

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


