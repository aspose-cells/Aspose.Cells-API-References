---
title: "Класс SmartTag"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Markup.SmartTag class. Представляет смарт‑тег"
type: docs
url: /ru/net/aspose.cells.markup/smarttag/
---
## SmartTag class

Представляет смарт‑тег.

```csharp
public class SmartTag
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Deleted](../../aspose.cells.markup/smarttag/deleted/) { get; set; } | Указывает, удалён ли смарт‑тег. |
| [Name](../../aspose.cells.markup/smarttag/name/) { get; } | Получает имя смарт‑тега. |
| [Properties](../../aspose.cells.markup/smarttag/properties/) { get; set; } | Получает и задаёт свойства смарт‑тега. |
| [Uri](../../aspose.cells.markup/smarttag/uri/) { get; } | Получает URI пространства имён смарт‑тега. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetLink](../../aspose.cells.markup/smarttag/setlink/)(string, string) | Изменяет имя и URI пространства имён смарт‑тега. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class MarkupClassSmartTagDemo
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

            workbook.Save("SmartTagDemo.xlsx");
            Console.WriteLine("SmartTagDemo.xlsx created successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


