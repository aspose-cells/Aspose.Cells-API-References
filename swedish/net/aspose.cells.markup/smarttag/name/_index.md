---
title: "SmartTag.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTag-egenskap. Hämtar namnet på smart tag"
type: docs
url: /sv/net/aspose.cells.markup/smarttag/name/
---
## SmartTag.Name property

Hämtar namnet på den smarta taggen.

```csharp
public string Name { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyNameDemo
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

            // Demonstrera Name-egenskapen (endast läsoperation)
            Console.WriteLine("SmartTag Name: " + smartTag.Name);

            // Spara arbetsboken
            workbook.Save("SmartTagNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


