---
title: "BuiltInDocumentPropertyCollection.LinksUpToDate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "BuiltInDocumentPropertyCollection property. يشير إلى ما إذا كانت الروابط التشعبية في المستند محدثة"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/linksuptodate/
---
## BuiltInDocumentPropertyCollection.LinksUpToDate property

يشير إلى ما إذا كانت الروابط التشعبية في المستند محدثة.

```csharp
public bool LinksUpToDate { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLinksUpToDateDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى مجموعة خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // قم بتعيين خاصية LinksUpToDate للإشارة إلى ما إذا كانت الروابط التشعبية حالية
            builtInProperties.LinksUpToDate = true;

            // أضف رابطًا تشعبيًا بسيطًا لتوضيح الخاصية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // احفظ المصنف
            workbook.Save("LinksUpToDateDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


