---
title: "SmartTagCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SmartTagCollection. تضيف علامة ذكية"
type: docs
url: /ar/net/aspose.cells.markup/smarttagcollection/add/
---
## SmartTagCollection.Add method

يضيف علامة ذكية.

```csharp
public int Add(string uri, string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| uri | String | يحدد URI مساحة الاسم للعلامة الذكية |
| name | String | يحدد اسم العلامة الذكية. |

### قيمة الإرجاع

فهرس الـ smart tag في القائمة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Added smart tag at index: " + tagIndex);
            workbook.Save("SmartTagCollectionAddExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


