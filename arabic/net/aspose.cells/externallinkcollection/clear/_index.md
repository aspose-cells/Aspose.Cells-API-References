---
title: "ExternalLinkCollection.Clear"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ExternalLinkCollection. تزيل جميع الروابط الخارجية"
type: docs
url: /ar/net/aspose.cells/externallinkcollection/clear/
---
## Clear() {#clear}

يزيل جميع الروابط الخارجية.

```csharp
public void Clear()
```

### ملاحظات

عند إزالة الروابط الخارجية، سيتم إزالة جميع الصيغ التي تشير إليها أيضًا لأن المراجع تصبح غير صالحة.

### انظر أيضًا

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Clear(bool) {#clear_1}

يزيل جميع الروابط الخارجية.

```csharp
public void Clear(bool updateReferencesAsLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| updateReferencesAsLocal | منطقي | ما إذا كان سيتم تحديث جميع مراجع الروابط الخارجية في الصيغ إلى مراجع المصنف الحالي نفسه. |

### ملاحظات

إذا كان من الضروري تحديث المراجع، فستتم تغيير مراجع الروابط الخارجية في الصيغ إلى المصنف الحالي عندما يكون ذلك ممكنًا. على سبيل المثال، الصيغة الأصلية لخلية ما هي "='externalsource.xlam'!customfunction()"، بعد إزالة الروابط الخارجية، ستصبح الصيغة "=customfunction()"؛ عندما تكون الصيغة الأصلية "='[externalsource.xlam]Sheet1'!$A$1"، وفقًا لما إذا كان هناك ورقة باسم "Sheet1" في المصنف الحالي: إذا كان صحيحًا، ستصبح الصيغة "=Sheet1!$A$1"؛ إذا كان خاطئًا، ستصبح الصيغة "=#REF!$A$1". إذا لم يكن من الضروري تحديث المراجع، فسيتم إزالة جميع الصيغ التي تحتوي على مراجع للروابط الخارجية أيضًا لأن تلك المراجع تصبح غير صالحة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkCollectionMethodClearWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // إضافة بعض الروابط الخارجية
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            Console.WriteLine("External links count before clear: " + externalLinks.Count);
            
            // مسح مع updateReferences = true
            externalLinks.Clear(true);
            Console.WriteLine("External links count after clear (updateReferences=true): " + externalLinks.Count);
            
            // أضف الروابط مرة أخرى
            externalLinks.Add("externalWorkbook.xlsx", new string[] { "Sheet1" });
            externalLinks.Add("anotherExternal.xlsx", new string[] { "Sheet1" });
            
            // مسح مع updateReferences = false
            externalLinks.Clear(false);
            Console.WriteLine("External links count after clear (updateReferences=false): " + externalLinks.Count);
        }
    }
}
```

### انظر أيضًا

* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


