---
title: "Sınıf SmartTag"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Markup.SmartTag sınıfı. Bir akıllı etiketi temsil eder"
type: docs
url: /tr/net/aspose.cells.markup/smarttag/
---
## SmartTag class

Akıllı bir etiketi temsil eder.

```csharp
public class SmartTag
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Deleted](../../aspose.cells.markup/smarttag/deleted/) { get; set; } | Akıllı etiketin silinip silinmediğini gösterir. |
| [Name](../../aspose.cells.markup/smarttag/name/) { get; } | Akıllı etiketin adını alır. |
| [Properties](../../aspose.cells.markup/smarttag/properties/) { get; set; } | Akıllı etiketin özelliklerini alır ve ayarlar. |
| [Uri](../../aspose.cells.markup/smarttag/uri/) { get; } | Akıllı etiketin ad alanı URI'sını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetLink](../../aspose.cells.markup/smarttag/setlink/)(string, string) | Akıllı etiketin adını ve ad alanı URI'sını değiştir. |

### Örnekler

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

### Ayrıca Bakınız

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


