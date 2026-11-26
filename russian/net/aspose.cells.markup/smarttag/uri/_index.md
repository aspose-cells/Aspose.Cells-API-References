---
title: "SmartTag.Uri"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SmartTag. Получает URI пространства имён умного тега"
type: docs
url: /ru/net/aspose.cells.markup/smarttag/uri/
---
## SmartTag.Uri property

Получает URI пространства имён смарт‑тега.

```csharp
public string Uri { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyUriDemo
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

            // Отобразить значение свойства Uri (операция только для чтения)
            Console.WriteLine("SmartTag Uri: " + smartTag.Uri);

            // Продемонстрировать другие свойства
            Console.WriteLine("SmartTag Name: " + smartTag.Name);

            // Сохраните книгу
            workbook.Save("SmartTagUriDemo.xlsx");
        }
    }
}
```

### См. также

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


