---
title: "Klass SmartTag"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Markup.SmartTag-klass. Representerar en smart tagg"
type: docs
url: /sv/net/aspose.cells.markup/smarttag/
---
## SmartTag class

Representerar en smart tagg.

```csharp
public class SmartTag
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Deleted](../../aspose.cells.markup/smarttag/deleted/) { get; set; } | Anger om den smarta taggen är raderad. |
| [Name](../../aspose.cells.markup/smarttag/name/) { get; } | Hämtar namnet på den smarta taggen. |
| [Properties](../../aspose.cells.markup/smarttag/properties/) { get; set; } | Hämtar och sätter egenskaperna för den smarta taggen. |
| [Uri](../../aspose.cells.markup/smarttag/uri/) { get; } | Hämtar namnrymdens URI för den smarta taggen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [SetLink](../../aspose.cells.markup/smarttag/setlink/)(string, string) | Ändra namnet och namnrymdens URI för den smarta taggen. |

### Exempel

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

### Se även

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


