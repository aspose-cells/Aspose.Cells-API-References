---
title: "SmartTagCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SmartTagCollection. Возвращает объект SmartTag по указанному индексу"
type: docs
url: /ru/net/aspose.cells.markup/smarttagcollection/item/
---
## SmartTagCollection indexer

Получает объект [`SmartTag`](../../smarttag/) по указанному индексу

```csharp
public SmartTag this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс. |

### Возвращаемое значение

возвращает объект [`SmartTag`](../../smarttag/).

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Description", "Aspose.Cells SmartTag");

            // Продемонстрировать использование свойства Item
            SmartTagProperty authorProperty = properties["Author"];
            Console.WriteLine($"Property 'Author' value: {authorProperty.Value}");

            workbook.Save("SmartTagPropertyDemo.xlsx");
            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### См. также

* class [SmartTag](../../smarttag/)
* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


