---
title: "فئة SensitivityLabelCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Metas.SensitivityLabelCollection. تمثل قائمة تصنيفات الحساسية"
type: docs
url: /ar/net/aspose.cells.metas/sensitivitylabelcollection/
---
## SensitivityLabelCollection class

يمثل قائمة تصنيفات الحساسية.

```csharp
public class SensitivityLabelCollection : CollectionBase<SensitivityLabel>
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [SensitivityLabelCollection](sensitivitylabelcollection/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells.metas/sensitivitylabelcollection/add/)(string, bool, SensitivityLabelAssignmentType, string, SensitivityLabelMarkType) | يضيف تصنيف حساسية. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SensitivityLabel) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SensitivityLabel, IComparer&lt;SensitivityLabel&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, SensitivityLabel, IComparer&lt;SensitivityLabel&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(SensitivityLabel) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SensitivityLabel[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SensitivityLabel[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, SensitivityLabel[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;SensitivityLabel&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;SensitivityLabel&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;SensitivityLabel&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;SensitivityLabel&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;SensitivityLabel&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SensitivityLabel) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SensitivityLabel, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SensitivityLabel, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SensitivityLabel) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SensitivityLabel, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SensitivityLabel, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelCollectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نسخة من فئة SensitivityLabelCollection
            SensitivityLabelCollection labels = new SensitivityLabelCollection();

            // إضافة تصنيفات حساسية بتكوينات مختلفة
            int index1 = labels.Add(
                id: "cb353f78-2f72-4d20-a5ca-ee47c4a5e7e1",
                isEnabled: true,
                methodType: SensitivityLabelAssignmentType.Standard,
                siteId: "contoso.sharepoint.com",
                markType: SensitivityLabelMarkType.Header);

            int index2 = labels.Add(
                id: "e48007e5-f9ac-4f63-9edc-6ab9a312688f",
                isEnabled: false,
                methodType: SensitivityLabelAssignmentType.Privileged,
                siteId: "contoso.sharepoint.com",
                markType: SensitivityLabelMarkType.Footer);

            // تطبيق التصنيفات على بيانات تعريف المصنف
            // استخدام CustomDocumentProperties بدلاً من ذلك لأن BuiltInDocumentProperties لا يدعم SensitivityLabels
            workbook.CustomDocumentProperties.Add("SensitivityLabels", labels.ToString());

            // حفظ المصنف مع تصنيفات الحساسية
            workbook.Save("SensitivityLabelCollectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [SensitivityLabel](../sensitivitylabel/)
* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


