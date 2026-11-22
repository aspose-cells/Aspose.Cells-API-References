---
title: "DxfCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DxfCollection. تحصل على العنصر في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/dxfcollection/item/
---
## DxfCollection indexer

يحصل على العنصر في الفهرس المحدد.

```csharp
public Style this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس المحدد. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DxfCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى DxfCollection من المصنف
            DxfCollection dxfCollection = workbook.Worksheets.Dxfs;

            // إنشاء نمط جديد (لا يمكن الإضافة مباشرة إلى DxfCollection لأنه لا يحتوي على طريقة Add)
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            // يتم إضافة النمط تلقائيًا إلى المجموعة عند إنشائه

            // احصل على العنصر الأول من DxfCollection باستخدام خاصية Item
            Style firstStyle = dxfCollection[0];
            Console.WriteLine("First style font name: " + firstStyle.Font.Name);

            // قم بتعديل النمط عبر خاصية Item (نظرًا لأنها تُعيد مرجعًا)
            firstStyle.Font.Color = System.Drawing.Color.Red;
            firstStyle.Font.IsBold = true;

            // تحقق من التغيير
            Console.WriteLine("Modified style font color: " + dxfCollection[0].Font.Color);
            Console.WriteLine("Modified style font bold: " + dxfCollection[0].Font.IsBold);

            // طبق النمط على خلية لرؤية التأثير
            worksheet.Cells["A1"].PutValue("DxfCollection Property Item Demo");
            worksheet.Cells["A1"].SetStyle(dxfCollection[0]);

            // حفظ النتيجة
            workbook.Save("DxfCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [DxfCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


