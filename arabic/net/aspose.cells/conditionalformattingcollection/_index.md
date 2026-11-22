---
title: "الفئة ConditionalFormattingCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.ConditionalFormattingCollection. تغلف مجموعة من كائنات FormatCondition"
type: docs
url: /ar/net/aspose.cells/conditionalformattingcollection/
---
## ConditionalFormattingCollection class

يغلف مجموعة من كائنات [`FormatCondition`](../formatcondition/)

```csharp
public class ConditionalFormattingCollection : CollectionBase<FormatConditionCollection>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/conditionalformattingcollection/item/) { get; } | يحصل على عنصر FormatConditions في الفهرس المحدد. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells/conditionalformattingcollection/add/)() | يضيف FormatConditions إلى المجموعة. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FormatConditionCollection) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, FormatConditionCollection, IComparer&lt;FormatConditionCollection&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(FormatConditionCollection) |  |
| [Copy](../../aspose.cells/conditionalformattingcollection/copy/)(ConditionalFormattingCollection) | ينسخ التنسيق الشرطي. |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FormatConditionCollection[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FormatConditionCollection[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, FormatConditionCollection[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;FormatConditionCollection&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FormatConditionCollection) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FormatConditionCollection, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FormatConditionCollection, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FormatConditionCollection) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FormatConditionCollection, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FormatConditionCollection, int, int) |  |
| [RemoveArea](../../aspose.cells/conditionalformattingcollection/removearea/)(int, int, int, int) | إزالة جميع التنسيقات الشرطية في النطاق. |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingCollectionDemo
    {
        public static void ConditionalFormattingCollectionExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // احصل على التنسيق الشرطي
            ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;

            // يضيف تنسيقًا شرطيًا فارغًا
            int index = cformattings.Add();

            // احصل على التنسيق الشرطي المضاف حديثًا
            FormatConditionCollection fcs = cformattings[index];

            // يحدد نطاق التنسيق الشرطي.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            ca = new CellArea
            {
                StartRow = 1,
                EndRow = 1,
                StartColumn = 1,
                EndColumn = 1
            };
            fcs.AddArea(ca);

            // أضف شرطًا.
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");

            // يضبط لون الخلفية.
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // حفظ ملف Excel
            workbook.Save("ConditionalFormattingCollectionDemo.xlsx");
            workbook.Save("ConditionalFormattingCollectionDemo.pdf");
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [FormatConditionCollection](../formatconditioncollection/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


