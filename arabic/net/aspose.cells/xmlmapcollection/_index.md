---
title: "الفئة XmlMapCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.XmlMapCollection. مجموعة من كائنات XmlMap التي تمثل معلومات XmlMap"
type: docs
url: /ar/net/aspose.cells/xmlmapcollection/
---
## XmlMapCollection class

مجموعة من كائنات [`XmlMap`](../xmlmap/) التي تمثل معلومات XmlMap.

```csharp
public class XmlMapCollection : CollectionBase<XmlMap>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/xmlmapcollection/item/) { get; } | يحصل على خريطة XML وفق الفهرس المحدد. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells/xmlmapcollection/add/)(string) | أضف [`XmlMap`](../xmlmap/) باستخدام عنوان URL/المسار لملف xml/xsd. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(XmlMap) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(XmlMap, IComparer&lt;XmlMap&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, XmlMap, IComparer&lt;XmlMap&gt;) |  |
| [Clear](../../aspose.cells/xmlmapcollection/clear/#clear)() | يزيل جميع XmlMaps. (طريقتان) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(XmlMap) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(XmlMap[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(XmlMap[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, XmlMap[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;XmlMap&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;XmlMap&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;XmlMap&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;XmlMap&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;XmlMap&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;XmlMap&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;XmlMap&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;XmlMap&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;XmlMap&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;XmlMap&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(XmlMap) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(XmlMap, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(XmlMap, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(XmlMap) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(XmlMap, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(XmlMap, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlMapCollectionDemo
    {
        public static void XmlMapCollectionExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى XmlMapCollection من المصنف
            XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;

            // أضف XmlMap جديد إلى المجموعة
            int xmlMapIndex = xmlMaps.Add("sample.xml");

            // الوصول إلى XmlMap المضاف حديثًا
            XmlMap xmlMap = xmlMaps[xmlMapIndex];

            // اعرض عدد XmlMaps في المجموعة
            Console.WriteLine("Number of XmlMaps: " + xmlMaps.Count);

            // اضبط سعة XmlMapCollection
            xmlMaps.Capacity = 10;

            // امسح جميع XmlMaps من المجموعة
            xmlMaps.Clear();

            // احفظ المصنف
            workbook.Save("XmlMapCollectionExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [XmlMap](../xmlmap/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


