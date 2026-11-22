---
title: "SmartTagCollection.Row"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SmartTagCollection. تحصل على صف العلامات الذكية للخلية"
type: docs
url: /ar/net/aspose.cells.markup/smarttagcollection/row/
---
## SmartTagCollection.Row property

يحصل على صف العلامات الذكية للخلية.

```csharp
public int Row { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف علامة ذكية إلى الخلية A1 (الصف 0، العمود 0)
            worksheet.Cells["A1"].PutValue("Sample with SmartTag");
            int index = worksheet.SmartTagSetting.Add("A1");
            
            // احصل على SmartTagCollection للخلية A1
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // اعرض صف الخلية التي تحتوي على هذه العلامات الذكية
            Console.WriteLine("SmartTags are located at row: " + smartTags.Row);

            // ملاحظة: خاصية Row للقراءة فقط، لذا لا يمكننا تعيينها
            // smartTags.Row = 5; // سيتسبب هذا في خطأ تجميع

            // أضف علامة ذكية أخرى إلى الخلية B3 (الصف 2، العمود 1) لتوضيح صف مختلف
            worksheet.Cells["B3"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("B3");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at row: " + smartTags2.Row);

            // احفظ المصنف
            workbook.Save("SmartTagRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


