---
title: "BuiltInDocumentPropertyCollection.LastSavedUniversalTime"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "BuiltInDocumentPropertyCollection property. يحصل أو يضبط الوقت العالمي لآخر حفظ"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/lastsaveduniversaltime/
---
## BuiltInDocumentPropertyCollection.LastSavedUniversalTime property

يحصل أو يضبط الوقت العالمي للحفظ الأخير.

```csharp
public DateTime LastSavedUniversalTime { get; set; }
```

### ملاحظات

Aspose.Cells لا يقوم بتحديث هذه الخاصية عندما تقوم بتعديل المستند.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedUniversalTimeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى خصائص المستند المدمجة
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // قم بتعيين خاصية LastSavedUniversalTime
            DateTime utcNow = DateTime.UtcNow;
            builtInProperties.LastSavedUniversalTime = utcNow;

            // عرض القيمة المحددة
            Console.WriteLine("LastSavedUniversalTime set to: " + builtInProperties.LastSavedUniversalTime);

            // احفظ المصنف
            workbook.Save("LastSavedUniversalTimeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


