---
title: "BuiltInDocumentPropertyCollection.LastPrinted"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية BuiltInDocumentPropertyCollection. تحصل أو تضبط التاريخ عندما تم طباعة المستند آخر مرة في المنطقة الزمنية المحلية"
type: docs
url: /ar/net/aspose.cells.properties/builtindocumentpropertycollection/lastprinted/
---
## BuiltInDocumentPropertyCollection.LastPrinted property

يحصل أو يضبط التاريخ الذي تم فيه طباعة المستند آخر مرة بالتوقيت المحلي.

```csharp
public DateTime LastPrinted { get; set; }
```

### ملاحظات

إذا لم يُطبع المستند أبداً، فإن هذه الخاصية ستعيد DateTime.MinValue.

Aspose.Cells لا يقوم بتحديث هذه الخاصية عندما تقوم بتعديل المستند.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastPrintedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // تعيين خصائص المستند المدمجة
            workbook.BuiltInDocumentProperties.CreatedTime = DateTime.Now;
            workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now.AddDays(-1); // Set to yesterday
            workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;

            // اعرض خاصية LastPrinted
            Console.WriteLine("Last printed: " + workbook.BuiltInDocumentProperties.LastPrinted);

            // احفظ المصنف
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


