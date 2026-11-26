---
title: "XmlMapCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод XmlMapCollection. Добавить XmlMap по URL/пути к файлу xml/xsd"
type: docs
url: /ru/net/aspose.cells/xmlmapcollection/add/
---
## XmlMapCollection.Add method

Добавьте [`XmlMap`](../../xmlmap/) по URL/пути к файлу xml/xsd.

```csharp
public int Add(string url)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| url | String | URL/путь к файлу xml/xsd. |

### Возвращаемое значение

[`XmlMap`](../../xmlmap/) object index.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            
            XmlMapCollection xmlMapCollection = wb.Worksheets.XmlMaps;
            
            // Добавьте XML‑карты, используя схему и XML‑файлы
            xmlMapCollection.Add("schema.xsd");
            xmlMapCollection.Add("xml.xml");
            
            wb.Save("twoXmlMaps.xlsx");
        }
    }
}
```

### См. также

* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


