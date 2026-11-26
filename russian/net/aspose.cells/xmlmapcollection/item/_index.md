---
title: "XmlMapCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlMapCollection. Получает xml map по указанному индексу"
type: docs
url: /ru/net/aspose.cells/xmlmapcollection/item/
---
## XmlMapCollection indexer

Получает xml‑map по указанному индексу.

```csharp
public XmlMap this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Возвращаемое значение

Эта xml карта

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Получить доступ к XmlMapCollection из рабочей книги
            XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;

            // Добавить новый XmlMap в коллекцию
            int xmlMapIndex = xmlMaps.Add("data.xsd");

            // Получите доступ к XmlMap с помощью свойства Item
            XmlMap xmlMap = xmlMaps[xmlMapIndex];

            // Отобразите имя XmlMap
            Console.WriteLine("XmlMap Name: " + xmlMap.Name);

            // Сохраните книгу
            workbook.Save("XmlMapCollectionExample.xlsx");
        }
    }
}
```

### См. также

* class [XmlMap](../../xmlmap/)
* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


