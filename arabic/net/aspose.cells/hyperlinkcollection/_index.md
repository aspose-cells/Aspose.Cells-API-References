---
title: "الفئة HyperlinkCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.HyperlinkCollection. تغلف مجموعة من كائنات Hyperlink."
type: docs
url: /ar/net/aspose.cells/hyperlinkcollection/
---
## HyperlinkCollection class

تغلف مجموعة من كائنات [`Hyperlink`](../hyperlink/).

```csharp
public class HyperlinkCollection : CollectionBase<Hyperlink>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/hyperlinkcollection/item/) { get; } | يحصل على عنصر [`Hyperlink`](../hyperlink/) في الفهرس المحدد. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add_1)(string, int, int, string) | يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا. |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add)(int, int, int, int, string) | يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا. |
| [Add](../../aspose.cells/hyperlinkcollection/add/#add_2)(string, string, string, string, string) | يضيف ارتباطًا تشعبيًا إلى خلية محددة أو نطاق من الخلايا. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Hyperlink) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [Clear](../../aspose.cells/hyperlinkcollection/clear/#clear)() | يمسح جميع الروابط التشعبية. (طريقتان) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Hyperlink) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Hyperlink[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Hyperlink[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Hyperlink[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Hyperlink&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Hyperlink, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Hyperlink, int, int) |  |
| [RemoveAt](../../aspose.cells/hyperlinkcollection/removeat/#removeat)(int) | إزالة الارتباط التشعبي في الفهرس المحدد في هذه المجموعة. (طريقتان) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HyperlinkCollectionDemo
    {
        public static void HyperlinkCollectionExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // الحصول على مرجع ورقة العمل التي تم إضافتها حديثًا بتمرير sheet index
            Worksheet worksheet = workbook.Worksheets[0];

            // الحصول على مجموعة الروابط التشعبية
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // إضافة ارتباط تشعبي إلى عنوان URL في الخلية "A1"
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // إضافة ارتباط تشعبي آخر إلى عنوان URL في الخلية "B1"
            hyperlinks.Add("B1", 1, 1, "http://www.example.com");

            // إضافة ارتباط تشعبي مع نطاق من الخلايا
            hyperlinks.Add("C1", 1, 2, "http://www.test.com");

            // إضافة ارتباط تشعبي بنص محدد للعرض وتلميح الشاشة
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            // إزالة الارتباط التشعبي الأول
            hyperlinks.RemoveAt(0);

            // مسح جميع الارتباطات التشعبية
            hyperlinks.Clear();

            // إضافة ارتباط تشعبي مرة أخرى لتوضيح الحفظ
            hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // حفظ ملف Excel
            workbook.Save("HyperlinkCollectionExample.xlsx");
            workbook.Save("HyperlinkCollectionExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


