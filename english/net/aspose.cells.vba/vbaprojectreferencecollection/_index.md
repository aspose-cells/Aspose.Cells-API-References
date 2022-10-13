---
title: VbaProjectReferenceCollection
second_title: Aspose.Cells for .NET API Reference
description: Represents all references of VBA project.
type: docs
weight: 6380
url: /net/aspose.cells.vba/vbaprojectreferencecollection/
---
## VbaProjectReferenceCollection class

Represents all references of VBA project.

```csharp
public class VbaProjectReferenceCollection : CollectionBase<VbaProjectReference>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count) { get; } |  |
| [Item](../../aspose.cells.vba/vbaprojectreferencecollection/item) { get; } | Get the reference in the list by the index. |
| [Item](../../aspose.cells/collectionbase-1/item) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [AddControlRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce)(string, string, string, string) | Add a reference to a twiddled type library and its extended type library. |
| [AddProjectRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce)(string, string, string) | Adds a reference to an external VBA project. |
| [AddRegisteredReference](../../aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference)(string, string) | Add a reference to an Automation type library. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch)(VbaProjectReference) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch)(VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch)(int, int, VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains)(VbaProjectReference) |  |
| [Copy](../../aspose.cells.vba/vbaprojectreferencecollection/copy)(VbaProjectReferenceCollection) | Copies references from other VBA project. |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto)(VbaProjectReference[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto)(VbaProjectReference[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto)(int, VbaProjectReference[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists)(Predicate&lt;VbaProjectReference&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex)(int, Predicate&lt;VbaProjectReference&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex)(int, int, Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex)(Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex)(int, Predicate&lt;VbaProjectReference&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex)(int, int, Predicate&lt;VbaProjectReference&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof)(VbaProjectReference) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof)(VbaProjectReference, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof)(VbaProjectReference, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof)(VbaProjectReference) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof)(VbaProjectReference, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof)(VbaProjectReference, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat)(int) |  |

### Examples

```csharp

[C#]

//Instantiating a Workbook object
Workbook workbook = new Workbook();
 // Init VBA project.
VbaProject vbaProject = workbook.VbaProject;
// Add vba project reference
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//Saving the Excel file
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Init VBA project.
Dim vbaProject as VbaProject  = workbook.VbaProject
'Add vba project reference
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
'Saving the Excel file
workbook.Save("book1.xlsm")
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [VbaProjectReference](../vbaprojectreference)
* namespace [Aspose.Cells.Vba](../../aspose.cells.vba)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
