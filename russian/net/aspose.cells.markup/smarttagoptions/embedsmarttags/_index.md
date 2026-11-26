---
title: "SmartTagOptions.EmbedSmartTags"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SmartTagOptions. Указывает, сохраняются ли смарт‑теги вместе с рабочей книгой"
type: docs
url: /ru/net/aspose.cells.markup/smarttagoptions/embedsmarttags/
---
## SmartTagOptions.EmbedSmartTags property

Указывает, сохранять ли смарт‑теги вместе с книгой.

```csharp
public bool EmbedSmartTags { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagOptionsPropertyEmbedSmartTagsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagOptions smartTagOptions = new SmartTagOptions();
            Console.WriteLine("Current EmbedSmartTags value: " + smartTagOptions.EmbedSmartTags);

            smartTagOptions.EmbedSmartTags = true;
            // SmartTagOptions теперь правильно используется, если это требуется API, хотя присвоение workbook.Settings недопустимо

            Console.WriteLine("after setting value: Current EmbedSmartTags value: " + smartTagOptions.EmbedSmartTags);

            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("New York");

            // Доступ к SmartTags через SmartTagSetting
            int index = worksheet.SmartTagSetting.Add(cell.Name);
            SmartTagCollection smartTagCollection = worksheet.SmartTagSetting[index];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags#place", "Place");
            SmartTag smartTag = smartTagCollection[tagIndex];
            smartTag.Properties.Add("State", "NY");
            // Используйте свойства для установки LinkedCell
            smartTag.Properties.Add("LinkedCell", cell.Name);

            workbook.Save("PropertyEmbedSmartTagsDemo.xlsx");
        }
    }
}
```

### См. также

* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


