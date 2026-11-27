---
title: "SmartTag.Uri"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTag-egenskap. Hämtar namnrymdens URI för smart tag"
type: docs
url: /sv/net/aspose.cells.markup/smarttag/uri/
---
## SmartTag.Uri property

Hämtar namnrymdens URI för den smarta taggen.

```csharp
public string Uri { get; }
```

### Exempel

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

            // Visa Uri-egenskapens värde (endast läsoperation)
            Console.WriteLine("SmartTag Uri: " + smartTag.Uri);

            // Demonstrera andra egenskaper
            Console.WriteLine("SmartTag Name: " + smartTag.Name);

            // Spara arbetsboken
            workbook.Save("SmartTagUriDemo.xlsx");
        }
    }
}
```

### Se även

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


