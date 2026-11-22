---
title: "الفئة ColumnCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ColumnCollection. مجموعة من كائنات Column التي تمثل إعدادات الأعمدة الفردية في ورقة العمل. كائن Column يمثل فقط الإعدادات مثل عرض العمود، الأنماط، إلخ للعمود بأكمله ولا علاقة له بوجود خلايا غير فارغة أو عدمها في العمود المقابل. وCount هذه المجموعة يمثل فقط عدد كائنات Column التي تم إنشاؤها في هذه المجموعة ولا علاقة له بوجود خلايا غير فارغة أو عدمها في ورقة العمل."
type: docs
url: /ar/net/aspose.cells/columncollection/
---
## ColumnCollection class

مجموعة من كائنات [`Column`](../column/) التي تمثل الأعمدة (الإعدادات) الفردية في ورقة العمل. كائن Column يمثل فقط الإعدادات مثل عرض العمود، الأنماط، إلخ للعمود بأكمله ولا علاقة له بوجود خلايا غير فارغة (بيانات) أو عدمها في العمود المقابل. و\"Count\" لهذه المجموعة يمثل فقط عدد كائنات Column التي تم إنشاؤها في هذه المجموعة، ولا علاقة له بوجود خلايا غير فارغة (بيانات) أو عدمها في ورقة العمل.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/columncollection/item/) { get; } | يحصل على كائن [`Column`](../column/) حسب فهرس العمود. سيتم إنشاء كائن Column للفهرس المحدد إذا لم يكن موجودًا مسبقًا. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Column) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Column, IComparer&lt;Column&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Column, IComparer&lt;Column&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Column) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Column[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Column[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Column[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Column&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Column&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Column&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Column&gt;) |  |
| [GetByIndex](../../aspose.cells/columncollection/getbyindex/)(int) | (**Obsolete.**) يحصل على كائن العمود حسب الفهرس. |
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex/)(int) | يحصل على كائن [`Column`](../column/) حسب الموقع في القائمة. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnCollectionDemo
    {
        public static void ColumnCollectionExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // الحصول على مرجع ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة نمط جديد إلى المصنف
            Style style = workbook.CreateStyle();

            // تعيين لون الخلفية إلى الأزرق
            style.ForegroundColor = Color.Blue;

            // تعيين نمط الخلفية
            style.Pattern = BackgroundType.Solid;

            // علامة النمط الجديد
            StyleFlag styleFlag = new StyleFlag();

            // ضبط جميع الأنماط
            styleFlag.All = true;

            // تغيير العرض الافتراضي لأول عشرة أعمدة
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells.Columns[i].Width = 20;
            }

            // احصل على Column بتنسيق غير افتراضي
            ColumnCollection columns = worksheet.Cells.Columns;

            foreach (Column column in columns)
            {
                // تطبيق النمط على أول عشرة أعمدة
                column.ApplyStyle(style, styleFlag);
            }

            // حفظ ملف Excel
            workbook.Save("ColumnCollectionExample.xlsx");
            workbook.Save("ColumnCollectionExample.pdf");
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Column](../column/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


