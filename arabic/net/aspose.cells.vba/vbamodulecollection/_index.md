---
title: "الفئة VbaModuleCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Vba.VbaModuleCollection class. يمثل قائمة VbaModule"
type: docs
url: /ar/net/aspose.cells.vba/vbamodulecollection/
---
## VbaModuleCollection class

يمثل قائمة [`VbaModule`](../vbamodule/)

```csharp
public class VbaModuleCollection : CollectionBase<VbaModule>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.vba/vbamodulecollection/item/) { get; } | يسترجع [`VbaModule`](../vbamodule/) في القائمة حسب الفهرس. (2 مؤشرات) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells.vba/vbamodulecollection/add/#add_1)(Worksheet) | يضيف وحدة لورقة عمل. |
| [Add](../../aspose.cells.vba/vbamodulecollection/add/#add)(VbaModuleType, string) | يضيف وحدة. |
| [AddDesignerStorage](../../aspose.cells.vba/vbamodulecollection/adddesignerstorage/)(string, byte[]) |  |
| [AddUserForm](../../aspose.cells.vba/vbamodulecollection/adduserform/)(string, string, byte[]) | إدراج نموذج مستخدم في مشروع VBA. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VbaModule) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(VbaModule, IComparer&lt;VbaModule&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, VbaModule, IComparer&lt;VbaModule&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(VbaModule) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VbaModule[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(VbaModule[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, VbaModule[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;VbaModule&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;VbaModule&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;VbaModule&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;VbaModule&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;VbaModule&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;VbaModule&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;VbaModule&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;VbaModule&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;VbaModule&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;VbaModule&gt;) |  |
| [GetDesignerStorage](../../aspose.cells.vba/vbamodulecollection/getdesignerstorage/)(string) | يمثل بيانات المصمم. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(VbaModule, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(VbaModule, int, int) |  |
| [Remove](../../aspose.cells.vba/vbamodulecollection/remove/#remove_1)(string) | إزالة الوحدة بالاسم |
| [Remove](../../aspose.cells.vba/vbamodulecollection/remove/#remove)(Worksheet) | يزيل وحدة لورقة عمل. |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaClassVbaModuleCollectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى مشروع VBA
            VbaProject vbaProject = workbook.VbaProject;
            
            // إضافة وحدة فئة جديدة
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestClass");
            
            // الحصول على الوحدة المضافة وإضافة بعض الشيفرة
            VbaModule module = vbaProject.Modules[index];
            module.Codes = "Public Sub TestMethod()\r\n    MsgBox \"Hello from VBA!\"\r\nEnd Sub";
            
            // حفظ كدفتر عمل يدعم الماكرو
            workbook.Save("VbaModuleCollectionDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [VbaModule](../vbamodule/)
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../)


