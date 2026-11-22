---
title: "الفئة NameCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.NameCollection. تمثل مجموعة من جميع كائنات Name في جدول البيانات"
type: docs
url: /ar/net/aspose.cells/namecollection/
---
## NameCollection class

تمثل مجموعة من جميع كائنات [`Name`](../name/) في جدول البيانات.

```csharp
public class NameCollection : CollectionBase<Name>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/namecollection/item/) { get; } | يحصل على عنصر [`Name`](../name/) في الفهرس المحدد. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells/namecollection/add/)(string) | يعرف اسمًا جديدًا. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name, IComparer&lt;Name&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Name, IComparer&lt;Name&gt;) |  |
| [Clear](../../aspose.cells/namecollection/clear/#clear)() | إزالة جميع الأسماء المعرفة التي لا يتم الإشارة إليها من قبل الصيغ ومصدر البيانات. إذا تم الإشارة إلى الاسم المعرفة، نقوم فقط بتعيين Name.ReferTo إلى null وإخفائه. (2 methods) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Name) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Name[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Name&gt;) |  |
| [Filter](../../aspose.cells/namecollection/filter/)(NameScopeType, int) | يحصل على جميع الأسماء المعرفة حسب النطاق. |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Name&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int, int) |  |
| [Remove](../../aspose.cells/namecollection/remove/#remove)(string) | إزالة الاسم. |
| [Remove](../../aspose.cells/namecollection/remove/#remove_1)(string[]) | إزالة مصفوفة من الأسماء |
| [RemoveAt](../../aspose.cells/namecollection/removeat/#removeat)(int) | إزالة الاسم عند الفهرس المحدد. (طريقتان) |
| [RemoveDuplicateNames](../../aspose.cells/namecollection/removeduplicatenames/)() | إزالة الأسماء المعرفة المكررة |
| [Sort](../../aspose.cells/namecollection/sort/)() | ترتيب الأسماء المعرفة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionDemo
    {
        public static void NameCollectionExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى مجموعة أوراق العمل
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // الوصول إلى مجموعة الأسماء
            NameCollection names = worksheets.Names;
            
            // إضافة اسم جديد إلى المجموعة
            int nameIndex = names.Add("MyNamedRange");
            Name name = names[nameIndex];
            
            // تعيين خاصية refers to للاسم
            name.RefersTo = "=Sheet1!$A$1:$A$10";
            
            // الوصول إلى خصائص الاسم وتعديلها
            name.Comment = "This is a named range for demonstration.";
            name.IsVisible = true;
            
            // إضافة اسم آخر
            int anotherNameIndex = names.Add("AnotherNamedRange");
            Name anotherName = names[anotherNameIndex];
            anotherName.RefersTo = "=Sheet1!$B$1:$B$10";
            
            // إزالة اسم بالنص
            names.Remove("AnotherNamedRange");
            
            // إزالة اسم بالفهرس
            names.RemoveAt(nameIndex);
            
            // مسح جميع الأسماء
            names.Clear();
            
            // احفظ المصنف
            workbook.Save("NameCollectionExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Name](../name/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


