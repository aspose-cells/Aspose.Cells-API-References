---
title: "WebExtensionPropertyCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WebExtensionPropertyCollection. تضيف خاصية web extension"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionpropertycollection/add/
---
## WebExtensionPropertyCollection.Add method

يضيف خاصية امتداد الويب.

```csharp
public int Add(string name, string value)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الخاصية. |
| القيمة | String | قيمة الخاصية. |

### قيمة الإرجاع

فهرس الخاصية المضافة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionPropertyCollectionMethodAddWithStringStringDemo
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
            
            // إظهار طريقة Add مع معلمات (String, String)
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            
            workbook.Save("WebExtensionExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


