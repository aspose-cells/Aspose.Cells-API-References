---
title: "Klasse SmartTag"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Markup.SmartTag Klasse. Stellt ein Smart‑Tag dar."
type: docs
url: /de/net/aspose.cells.markup/smarttag/
---
## SmartTag class

Stellt ein SmartTag dar.

```csharp
public class SmartTag
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Deleted](../../aspose.cells.markup/smarttag/deleted/) { get; set; } | Gibt an, ob das Smart‑Tag gelöscht ist. |
| [Name](../../aspose.cells.markup/smarttag/name/) { get; } | Liest den Namen des Smart‑Tags. |
| [Properties](../../aspose.cells.markup/smarttag/properties/) { get; set; } | Liest und legt die Eigenschaften des Smart‑Tags fest. |
| [Uri](../../aspose.cells.markup/smarttag/uri/) { get; } | Liest den Namespace‑URI des Smart‑Tags. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetLink](../../aspose.cells.markup/smarttag/setlink/)(string, string) | Ändere den Namen und den Namespace‑URI des Smart‑Tags. |

### Beispiele

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

### Siehe auch

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


