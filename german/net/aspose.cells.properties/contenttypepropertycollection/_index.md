---
title: ContentTypePropertyCollection
second_title: Aspose.Cells für .NET-API-Referenz
description: Eine Sammlung vonContentTypeProperty./contenttypeproperty Objekte die zusätzliche Informationen darstellen.
type: docs
weight: 4820
url: /de/net/aspose.cells.properties/contenttypepropertycollection/
---
## ContentTypePropertyCollection class

Eine Sammlung von[`ContentTypeProperty`](../contenttypeproperty) Objekte, die zusätzliche Informationen darstellen.

```csharp
public class ContentTypePropertyCollection : CollectionBase<ContentTypeProperty>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells.properties/contenttypepropertycollection/item) { get; } | Ruft die Eigenschaft des Inhaltstyps nach dem spezifischen Index ab. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.properties/contenttypepropertycollection/add#add)(string, string) | Fügt Inhaltstyp-Eigenschaftsinformationen hinzu. |
| [Add](../../aspose.cells.properties/contenttypepropertycollection/add#add_1)(string, string, string) | Fügt Inhaltstyp-Eigenschaftsinformationen hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(ContentTypeProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(ContentTypeProperty, IComparer&lt;ContentTypeProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, ContentTypeProperty, IComparer&lt;ContentTypeProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase`1/clear)() |  |
| [Contains](../../aspose.cells/collectionbase`1/contains)(ContentTypeProperty) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(ContentTypeProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(ContentTypeProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, ContentTypeProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;ContentTypeProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ContentTypeProperty) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ContentTypeProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(ContentTypeProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ContentTypeProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ContentTypeProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(ContentTypeProperty, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase`1/removeat)(int) |  |

### Beispiele

```csharp

[C#]

//Instanziieren eines Workbook-Objekts
Workbook workbook = new Workbook();
//Eine neue Eigenschaft hinzufügen.
 workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
//Excel-Datei speichern
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instanziieren eines Workbook-Objekts
Dim workbook As Workbook = New Workbook()
'Fügen Sie eine neue Eigenschaft hinzu.
 workbook.ContentTypeProperties.Add("Admin", "Aspose", "text")
'Speichern Sie die Excel-Datei
workbook.Save("book1.xlsm")
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [ContentTypeProperty](../contenttypeproperty)
* namensraum [Aspose.Cells.Properties](../../aspose.cells.properties)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
