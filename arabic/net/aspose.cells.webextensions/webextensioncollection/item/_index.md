---
title: "WebExtensionCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionCollection. تحصل على ملحق الويب حسب الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensioncollection/item/
---
## WebExtensionCollection indexer

يحصل على امتداد الويب حسب الفهرس المحدد.

```csharp
public WebExtension this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### قيمة الإرجاع

ملحق الويب.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احصل على مجموعة ملحقات الويب
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            
            // أضف ملحق مشغل فيديو ويب
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            webExt.Reference.Id = "youtube";
            webExt.Reference.StoreName = "youtube.com";
            webExt.Properties.Add("videoUrl", "https://www.youtube.com/watch?v=z0hFbzPPfm8");
            
            // أضف شكلاً لحمل ملحق الويب
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 410, 730, 0, 0);
            
            // عيّن ملحق الويب إلى الشكل
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            // احفظ المصنف
            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WebExtension](../../webextension/)
* class [WebExtensionCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


