---
title: "الفئة SmartTag"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Markup.SmartTag. تمثل علامة ذكية."
type: docs
url: /ar/net/aspose.cells.markup/smarttag/
---
## SmartTag class

يمثل علامة ذكية.

```csharp
public class SmartTag
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Deleted](../../aspose.cells.markup/smarttag/deleted/) { get; set; } | يشير إلى ما إذا كانت العلامة الذكية محذوفة. |
| [Name](../../aspose.cells.markup/smarttag/name/) { get; } | يحصل على اسم العلامة الذكية. |
| [Properties](../../aspose.cells.markup/smarttag/properties/) { get; set; } | يحصل على خصائص العلامة الذكية ويضبطها. |
| [Uri](../../aspose.cells.markup/smarttag/uri/) { get; } | يحصل على URI مساحة الاسم للعلامة الذكية. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetLink](../../aspose.cells.markup/smarttag/setlink/)(string, string) | غيّر الاسم وURI مساحة الاسم للعلامة الذكية. |

### أمثلة

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

### انظر أيضًا

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


