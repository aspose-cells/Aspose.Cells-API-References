---
title: "WebExtensionReference.Id"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionReference. تحصل وتضبط المعرف المرتبط بـ Office Addin داخل مزود الفهرس. يجب أن يكون المعرف فريدًا داخل مزود الفهرس"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionreference/id/
---
## WebExtensionReference.Id property

يحصل ويضبط المعرف المرتبط بإضافة Office داخل موفر الفهرس. يجب أن يكون المعرف فريدًا داخل موفر الفهرس.

```csharp
public string Id { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WebExtensionReferencePropertyIdDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            
            // تعيين خاصية Id والخصائص المرجعية الأخرى
            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0";
            webExt.Reference.StoreName = "en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            
            // إضافة خصائص امتداد الويب
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            // إضافة الشكل وربط امتداد الويب
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;

            // حفظ والتحقق
            workbook.Save("web_extension_demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionReference](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


