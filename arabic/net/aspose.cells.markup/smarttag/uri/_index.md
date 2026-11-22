---
title: "SmartTag.Uri"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SmartTag. يحصل على URI مساحة الاسم للعلامة الذكية"
type: docs
url: /ar/net/aspose.cells.markup/smarttag/uri/
---
## SmartTag.Uri property

يحصل على URI مساحة الاسم للعلامة الذكية.

```csharp
public string Uri { get; }
```

### أمثلة

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

            // عرض قيمة خاصية Uri (عملية قراءة فقط)
            Console.WriteLine("SmartTag Uri: " + smartTag.Uri);

            // إظهار خصائص أخرى
            Console.WriteLine("SmartTag Name: " + smartTag.Name);

            // احفظ المصنف
            workbook.Save("SmartTagUriDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


