---
title: VbaProjectReferenceCollection
second_title: Aspose.Cells for .NET API Referansı
description: VBA projesinin tüm başvurularını temsil eder.
type: docs
weight: 6290
url: /tr/net/aspose.cells.vba/vbaprojectreferencecollection/
---
## VbaProjectReferenceCollection class

VBA projesinin tüm başvurularını temsil eder.

```csharp
public class VbaProjectReferenceCollection : CollectionBase<VbaProjectReference>
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.vba/vbaprojectreferencecollection/item) { get; } | Listedeki referansı dizine göre alın. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [AddControlRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce)(string, string, string, string) | Döndürülmüş tür kitaplığına ve genişletilmiş tür kitaplığına bir başvuru ekleyin. |
| [AddProjectRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce)(string, string, string) | Harici bir VBA projesine başvuru ekler. |
| [AddRegisteredReference](../../aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference)(string, string) | Otomasyon türü kitaplığına başvuru ekleyin. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(VbaProjectReference) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(VbaProjectReference) |  |
| [Copy](../../aspose.cells.vba/vbaprojectreferencecollection/copy)(VbaProjectReferenceCollection) | Diğer VBA projesinden referansları kopyalar. |
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

### Örnekler

```csharp

[C#]

//Bir Çalışma Kitabı nesnesini başlatma
Workbook workbook = new Workbook();
 // VBA projesini başlat.
VbaProject vbaProject = workbook.VbaProject;
// vba proje referansı ekle
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//Excel dosyasını kaydetme
workbook.Save("book1.xlsm");

 [Visual Basic]

'Bir Çalışma Kitabı nesnesini başlatma
Dim workbook As Workbook = New Workbook()
'VBA projesini başlatın.
Dim vbaProject as VbaProject  = workbook.VbaProject
'vba proje referansı ekleyin
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
'Excel dosyasını kaydetme
workbook.Save("book1.xlsm")
```

### Ayrıca bakınız

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [VbaProjectReference](../vbaprojectreference)
* ad alanı [Aspose.Cells.Vba](../../aspose.cells.vba)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
