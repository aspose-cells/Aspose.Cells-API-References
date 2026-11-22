---
title: "SmartTagCollection.Column"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SmartTagCollection. تحصل على عمود العلامات الذكية للخلية"
type: docs
url: /ar/net/aspose.cells.markup/smarttagcollection/column/
---
## SmartTagCollection.Column property

يحصل على عمود العلامات الذكية للخلية.

```csharp
public int Column { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف علامة ذكية إلى الخلية C5 (الصف 4، العمود 2)
            worksheet.Cells["C5"].PutValue("SmartTag Demo");
            int index = worksheet.SmartTagSetting.Add("C5");
            
            // احصل على SmartTagCollection للخلية C5
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // اعرض عمود الخلية التي تحتوي على هذه العلامات الذكية
            Console.WriteLine("SmartTags are located at column: " + smartTags.Column);

            // أضف علامة ذكية أخرى إلى الخلية E2 (الصف 1، العمود 4) لتوضيح عمود مختلف
            worksheet.Cells["E2"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("E2");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at column: " + smartTags2.Column);

            // احفظ المصنف
            workbook.Save("SmartTagColumnDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


