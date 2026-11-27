---
title: "SmartTag.Deleted"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTag-egenskap. Anger om smart tag är raderad"
type: docs
url: /sv/net/aspose.cells.markup/smarttag/deleted/
---
## SmartTag.Deleted property

Anger om den smarta taggen är raderad.

```csharp
public bool Deleted { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyDeletedDemo
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

            Console.WriteLine("Initial Deleted value: " + smartTag.Deleted);

            // Ställ in egenskapen Deleted till true
            smartTag.Deleted = true;
            Console.WriteLine("After setting Deleted: " + smartTag.Deleted);

            // Spara arbetsboken
            workbook.Save("SmartTagDeletedDemo.xlsx");

        }
    }
}
```

### Se även

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


