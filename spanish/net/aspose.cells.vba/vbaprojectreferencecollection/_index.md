---
title: VbaProjectReferenceCollection
second_title: Referencia de API de Aspose.Cells para .NET
description: Representa todas las referencias del proyecto VBA.
type: docs
weight: 6290
url: /es/net/aspose.cells.vba/vbaprojectreferencecollection/
---
## VbaProjectReferenceCollection class

Representa todas las referencias del proyecto VBA.

```csharp
public class VbaProjectReferenceCollection : CollectionBase<VbaProjectReference>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.vba/vbaprojectreferencecollection/item) { get; } | Obtener la referencia en la lista por el índice. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddControlRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce)(string, string, string, string) | Agregue una referencia a una biblioteca de tipos manipulados y su biblioteca de tipos extendida. |
| [AddProjectRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce)(string, string, string) | Agrega una referencia a un proyecto VBA externo. |
| [AddRegisteredReference](../../aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference)(string, string) | Agregar una referencia a una biblioteca de tipos de automatización. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(VbaProjectReference) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(VbaProjectReference) |  |
| [Copy](../../aspose.cells.vba/vbaprojectreferencecollection/copy)(VbaProjectReferenceCollection) | Copia referencias de otro proyecto VBA. |
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

### Ejemplos

```csharp

[C#]

// Instanciando un objeto Workbook
Workbook workbook = new Workbook();
 // Inicie el proyecto VBA.
VbaProject vbaProject = workbook.VbaProject;
// Agregar referencia de proyecto vba
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//Guardando el archivo de Excel
workbook.Save("book1.xlsm");

 [Visual Basic]

'Crear una instancia de un objeto Workbook
Dim workbook As Workbook = New Workbook()
'Inicie proyecto VBA.
Dim vbaProject as VbaProject  = workbook.VbaProject
'Agregar referencia de proyecto vba
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
'Guardar el archivo de Excel
workbook.Save("book1.xlsm")
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [VbaProjectReference](../vbaprojectreference)
* espacio de nombres [Aspose.Cells.Vba](../../aspose.cells.vba)
* asamblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
