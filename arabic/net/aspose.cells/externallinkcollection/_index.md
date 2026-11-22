---
title: "الفئة ExternalLinkCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ExternalLinkCollection. تمثل مجموعة الروابط الخارجية في مصنف"
type: docs
url: /ar/net/aspose.cells/externallinkcollection/
---
## ExternalLinkCollection class

يمثل مجموعة الروابط الخارجية في المصنف.

```csharp
public class ExternalLinkCollection : IEnumerable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.cells/externallinkcollection/count/) { get; } | يحصل على عدد العناصر الموجودة فعليًا في المجموعة. |
| [Item](../../aspose.cells/externallinkcollection/item/) { get; } | يحصل على العنصر [`ExternalLink`](../externallink/) في الفهرس المحدد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells/externallinkcollection/add/#add_1)(string, string[]) | يضيف رابطًا خارجيًا. |
| [Add](../../aspose.cells/externallinkcollection/add/#add)(DirectoryType, string, string[]) | إضافة رابط خارجي. |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear)() | يزيل جميع الروابط الخارجية. |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear_1)(bool) | يزيل جميع الروابط الخارجية. |
| [GetEnumerator](../../aspose.cells/externallinkcollection/getenumerator/)() | احصل على مُعدِّد يتنقل عبر هذه المجموعة. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat)(int) | يزيل الرابط الخارجي المحدد من المصنف. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat_1)(int, bool) | يزيل الرابط الخارجي المحدد من المصنف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExternalLinkCollectionDemo
    {
        public static void ExternalLinkCollectionExample()
        {
            // فتح ملف يحتوي على روابط خارجية
            Workbook workbook = new Workbook("ExternalLinkCollectionExample_original.xlsx");

            // احصل على مجموعة الروابط الخارجية
            ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;

            // عرض عدد الروابط الخارجية
            Console.WriteLine("Number of external links: " + externalLinks.Count);

            // تكرار عبر الروابط الخارجية وعرض مصادر البيانات الخاصة بها
            for (int i = 0; i < externalLinks.Count; i++)
            {
                ExternalLink link = externalLinks[i];
                Console.WriteLine("External Link " + i + " Data Source: " + link.DataSource);
            }

            // إضافة رابط خارجي جديد
            int newLinkIndex = externalLinks.Add("newLink.xls", new[] { "Sheet1" });
            Console.WriteLine("Added new external link at index: " + newLinkIndex);

            // تغيير مصدر البيانات للرابط الخارجي الأول
            if (externalLinks.Count > 0)
            {
                externalLinks[0].DataSource = "d:\\link.xlsx";
                Console.WriteLine("Updated data source of the first external link.");
            }

            // احفظ المصنف
            workbook.Save("ExternalLinkCollectionExample.xlsx");

            // مسح جميع الروابط الخارجية
            externalLinks.Clear();
            Console.WriteLine("Cleared all external links.");

            // احفظ المصنف بعد مسح الروابط الخارجية
            workbook.Save("ExternalLinkCollectionExample2.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


