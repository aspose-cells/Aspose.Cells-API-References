---
title: "الفئة WebExtension"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.WebExtensions.WebExtension. تمثل نسخة مكوّن Office"
type: docs
url: /ar/net/aspose.cells.webextensions/webextension/
---
## WebExtension class

يمثل مثيل Office Add-in.

```csharp
public class WebExtension
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AlterReferences](../../aspose.cells.webextensions/webextension/alterreferences/) { get; } | يحصل على قائمة بالمراجع المعدلة. |
| [Bindings](../../aspose.cells.webextensions/webextension/bindings/) { get; } | يحصل على جميع علاقات الربط بين مكوّن Office والبيانات في المستند. |
| [Id](../../aspose.cells.webextensions/webextension/id/) { get; set; } | يحصل ويضبط المعرف الفريد لنسخة مكوّن Office في المستند الحالي. |
| [IsFrozen](../../aspose.cells.webextensions/webextension/isfrozen/) { get; set; } | يشير إلى ما إذا كان المستخدم يمكنه التفاعل مع مكوّن Office أم لا. |
| [Properties](../../aspose.cells.webextensions/webextension/properties/) { get; } | يحصل على جميع خصائص الامتداد الويب. |
| [Reference](../../aspose.cells.webextensions/webextension/reference/) { get; } | احصل على المرجع الأساسي لمكوّن Office. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionsClassWebExtensionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            webExt.Reference.Id = "youtube";
            webExt.Reference.StoreName = "YouTube";
            
            webExt.Properties.Add("videoUrl", "https://www.youtube.com/watch?v=z0hFbzPPfm8");
            
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 410, 730);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            workbook.Save("WebExtensionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


