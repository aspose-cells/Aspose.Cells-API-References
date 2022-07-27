---
title: VbaProjectReferenceCollection
second_title: Aspose.Cells لمرجع .NET API
description: يمثل جميع مراجع مشروع VBA .
type: docs
weight: 6290
url: /ar/net/aspose.cells.vba/vbaprojectreferencecollection/
---
## VbaProjectReferenceCollection class

يمثل جميع مراجع مشروع VBA .

```csharp
public class VbaProjectReferenceCollection : CollectionBase<VbaProjectReference>
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.vba/vbaprojectreferencecollection/item) { get; } | احصل على المرجع في القائمة من خلال الفهرس . |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## طُرق

| اسم | وصف |
| --- | --- |
| [AddControlRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce)(string, string, string, string) | قم بإضافة مرجع إلى مكتبة نوع ملفوفة ومكتبة النوع الموسعة الخاصة بها. |
| [AddProjectRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce)(string, string, string) | إضافة مرجع إلى مشروع VBA خارجي. |
| [AddRegisteredReference](../../aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference)(string, string) | إضافة مرجع إلى مكتبة نوع التنفيذ التلقائي. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(VbaProjectReference) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(VbaProjectReference) |  |
| [Copy](../../aspose.cells.vba/vbaprojectreferencecollection/copy)(VbaProjectReferenceCollection) | نسخ مراجع من مشروع VBA آخر . |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(VbaProjectReference[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(VbaProjectReference[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, VbaProjectReference[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;VbaProjectReference&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;VbaProjectReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;VbaProjectReference&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(VbaProjectReference) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(VbaProjectReference, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(VbaProjectReference, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(VbaProjectReference) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(VbaProjectReference, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(VbaProjectReference, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### أمثلة

```csharp

[C#]

// إنشاء كائن مصنف
Workbook workbook = new Workbook();
 // التهيئة لمشروع VBA.
VbaProject vbaProject = workbook.VbaProject;
// إضافة مرجع مشروع vba
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
// حفظ ملف Excel
workbook.Save("book1.xlsm");

 [Visual Basic]

'إنشاء كائن مصنف
Dim workbook As Workbook = New Workbook()
'مشروع التهيئة VBA.
Dim vbaProject as VbaProject  = workbook.VbaProject
'أضف مرجع مشروع vba
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
'حفظ ملف Excel
workbook.Save("book1.xlsm")
```

### أنظر أيضا

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [VbaProjectReference](../vbaprojectreference)
* مساحة الاسم [Aspose.Cells.Vba](../../aspose.cells.vba)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
