---
title: "SmartTag.Name"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SmartTag özelliği. Akıllı etiketin adını alır."
type: docs
url: /tr/net/aspose.cells.markup/smarttag/name/
---
## SmartTag.Name property

Akıllı etiketin adını alır.

```csharp
public string Name { get; }
```

### Örnekler

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

            // Name özelliğini gösterin (yalnızca okuma işlemi).
            Console.WriteLine("SmartTag Name: " + smartTag.Name);

            // Çalışma kitabını kaydedin
            workbook.Save("SmartTagNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


