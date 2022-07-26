---
title: VbaProjectReferenceCollection
second_title: Référence de l'API Aspose.Cells pour .NET
description: Représente toutes les références du projet VBA.
type: docs
weight: 6290
url: /fr/net/aspose.cells.vba/vbaprojectreferencecollection/
---
## VbaProjectReferenceCollection class

Représente toutes les références du projet VBA.

```csharp
public class VbaProjectReferenceCollection : CollectionBase<VbaProjectReference>
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.vba/vbaprojectreferencecollection/item) { get; } | Obtenir la référence dans la liste par l'index. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Méthodes

| Nom | La description |
| --- | --- |
| [AddControlRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addcontrolrefrernce)(string, string, string, string) | Ajouter une référence à une bibliothèque de types modifiée et à sa bibliothèque de types étendue. |
| [AddProjectRefrernce](../../aspose.cells.vba/vbaprojectreferencecollection/addprojectrefrernce)(string, string, string) | Ajoute une référence à un projet VBA externe. |
| [AddRegisteredReference](../../aspose.cells.vba/vbaprojectreferencecollection/addregisteredreference)(string, string) | Ajouter une référence à une bibliothèque de types Automation. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(VbaProjectReference) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, VbaProjectReference, IComparer&lt;VbaProjectReference&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(VbaProjectReference) |  |
| [Copy](../../aspose.cells.vba/vbaprojectreferencecollection/copy)(VbaProjectReferenceCollection) | Copie les références d'un autre projet VBA. |
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

### Exemples

```csharp

[C#]

//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();
 // Initier le projet VBA.
VbaProject vbaProject = workbook.VbaProject;
// Ajouter une référence de projet vba
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
//Enregistrement du fichier Excel
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()
'Lancer le projet VBA.
Dim vbaProject as VbaProject  = workbook.VbaProject
'Ajouter une référence de projet vba
vbaProject.References.AddRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
'Enregistrement du fichier Excel
workbook.Save("book1.xlsm")
```

### Voir également

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [VbaProjectReference](../vbaprojectreference)
* espace de noms [Aspose.Cells.Vba](../../aspose.cells.vba)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
