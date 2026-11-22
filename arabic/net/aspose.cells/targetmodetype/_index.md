---
title: "تعداد TargetModeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.TargetModeType. يمثل نوع وضع الهدف"
type: docs
url: /ar/net/aspose.cells/targetmodetype/
---
## TargetModeType enumeration

يمثل نوع وضع الهدف.

```csharp
public enum TargetModeType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| External | `0` | رابط خارجي |
| FilePath | `1` | المسارات المحلية والكاملة للملفات أو المجلدات. |
| Email | `2` | البريد الإلكتروني. |
| CellReference | `3` | رابط على خلية أو نطاق مسمى. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTargetModeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة ارتباط تشعبي خارجي
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // احصل على الارتباط التشعبي وتحقق من TargetModeType الخاص به
            Hyperlink link = worksheet.Hyperlinks[0];
            Console.WriteLine("Hyperlink TargetModeType: " + link.LinkType);
            
            // حذف الارتباط التشعبي
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


