---
title: "SmartTag.Uri"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SmartTag özelliği. Akıllı etiketin ad alanı URI'sini alır"
type: docs
url: /tr/net/aspose.cells.markup/smarttag/uri/
---
## SmartTag.Uri property

Akıllı etiketin ad alanı URI'sını alır.

```csharp
public string Uri { get; }
```

### Örnekler

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

            // Uri özelliği değerini göster (yalnızca okuma işlemi)
            Console.WriteLine("SmartTag Uri: " + smartTag.Uri);

            // Diğer özellikleri göster
            Console.WriteLine("SmartTag Name: " + smartTag.Name);

            // Çalışma kitabını kaydedin
            workbook.Save("SmartTagUriDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


