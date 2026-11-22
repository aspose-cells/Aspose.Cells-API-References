---
title: "التعداد WebExtensionStoreType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.WebExtensions.WebExtensionStoreType. يمثل نوع المتجر للامتداد الويب"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionstoretype/
---
## WebExtensionStoreType enumeration

يمثل نوع المتجر ل web extension.

```csharp
public enum WebExtensionStoreType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| OMEX | `0` | يحدد أن نوع المتجر هو Office.com. |
| SPCatalog | `1` | يحدد أن نوع المتجر هو كتالوج SharePoint المؤسسي. |
| SPApp | `2` | يحدد أن نوع المتجر هو تطبيق ويب SharePoint. |
| Exchange | `3` | يحدد أن نوع المتجر هو خادم Exchange. |
| FileSystem | `4` | يحدد أن نوع المتجر هو مشاركة نظام ملفات. |
| Registry | `5` | يحدد أن نوع المتجر هو سجل النظام. |
| ExCatalog | `6` | يحدد أن نوع المتجر هو النشر المركزي عبر Exchange. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WebExtensionsClassWebExtensionStoreTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            
            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0";
            webExt.Reference.StoreName = "en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            
            webExt.Properties.Add("sku", "\"peoplebar-giant\"");
            webExt.Properties.Add("theme", "\"giant-redwhiteblack\"");
            webExt.Properties.Add("shape", "\"muscle-people\"");
            webExt.Properties.Add("layout-element-title", "\"NUMBERS ABOUT THE APP\"");
            
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;

            workbook.Save("WebExtensionStoreTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


