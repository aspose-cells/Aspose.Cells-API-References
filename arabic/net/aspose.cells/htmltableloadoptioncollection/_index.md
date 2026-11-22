---
title: "الفئة HtmlTableLoadOptionCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.HtmlTableLoadOptionCollection. تمثل خيارات الجدول عند استيراد HTML"
type: docs
url: /ar/net/aspose.cells/htmltableloadoptioncollection/
---
## HtmlTableLoadOptionCollection class

يمثل خيارات الجدول عند استيراد HTML.

```csharp
public class HtmlTableLoadOptionCollection : CollectionBase<HtmlTableLoadOption>
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [HtmlTableLoadOptionCollection](htmltableloadoptioncollection/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/htmltableloadoptioncollection/item/) { get; } | يحصل على العنصر [`HtmlTableLoadOption`](../htmltableloadoption/) في الفهرس المحدد. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [TableToListObject](../../aspose.cells/htmltableloadoptioncollection/tabletolistobject/) { get; set; } | يشير إلى ما إذا كان سيتم إنشاء كائنات قائمة من الجداول المستوردة. القيمة الافتراضية هي false. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add)(HtmlTableLoadOption) | (**Obsolete.**) يضيف HtmlTableLoadOption واحد إلى هذه المجموعة. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_1)(int) | أضف HtmlTableLoadOption إلى القائمة. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_4)(string) | أضف HtmlTableLoadOption إلى القائمة. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_2)(int, int) | أضف HtmlTableLoadOption إلى القائمة. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_5)(string, int) | أضف HtmlTableLoadOption إلى القائمة. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_3)(int, int, int) | أضف HtmlTableLoadOption إلى القائمة. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_6)(string, int, int) | أضف HtmlTableLoadOption إلى القائمة. |
| [AddTableLoadOption](../../aspose.cells/htmltableloadoptioncollection/addtableloadoption/)(HtmlTableLoadOption) | يضيف HtmlTableLoadOption واحد إلى هذه المجموعة. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(HtmlTableLoadOption) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, HtmlTableLoadOption[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionCollectionDemo
    {
        public static void HtmlTableLoadOptionCollectionExample()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();

            // إنشاء HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // الوصول إلى مثال HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // تعيين خاصية TableToListObject
            tableLoadOptions.TableToListObject = true;

            // إضافة HtmlTableLoadOption جديد حسب فهرس الجدول
            int index1 = tableLoadOptions.Add(0);

            // إضافة HtmlTableLoadOption جديد حسب معرف الجدول
            int index2 = tableLoadOptions.Add("tableId");

            // إضافة HtmlTableLoadOption جديد حسب فهرس الجدول وفهرس الورقة المستهدفة
            int index3 = tableLoadOptions.Add(1, 1);

            // إضافة HtmlTableLoadOption جديد حسب معرف الجدول وفهرس الورقة المستهدفة
            int index4 = tableLoadOptions.Add("tableId2", 2);

            // إضافة HtmlTableLoadOption جديد حسب فهرس الجدول، فهرس الورقة المستهدفة، وفهرس الورقة الأصلية
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // إضافة HtmlTableLoadOption جديد حسب معرف الجدول، فهرس الورقة المستهدفة، وفهرس الورقة الأصلية
            int index6 = tableLoadOptions.Add("tableId3", 3, 1);

            // الوصول إلى HtmlTableLoadOption عند فهرس محدد
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // تعيين خصائص HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = "tableId";
            option.Name = "TableName";
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // تحميل ملف HTML إلى المصنف باستخدام خيارات التحميل
            workbook = new Workbook("HtmlTableLoadOptionCollectionExample_original.html", loadOptions);

            // احفظ المصنف
            workbook.Save("HtmlTableLoadOptionCollectionExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [HtmlTableLoadOption](../htmltableloadoption/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


