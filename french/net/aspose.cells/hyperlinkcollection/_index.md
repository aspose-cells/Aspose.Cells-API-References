---
title: HyperlinkCollection
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule une collection deHyperlink./hyperlink objets.
type: docs
weight: 3760
url: /fr/net/aspose.cells/hyperlinkcollection/
---
## HyperlinkCollection class

Encapsule une collection de[`Hyperlink`](../hyperlink) objets.

```csharp
public class HyperlinkCollection : CollectionBase<Hyperlink>
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [Item](../../aspose.cells/hyperlinkcollection/item) { get; } | Obtient le[`Hyperlink`](../hyperlink) élément à l'index spécifié. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |

## Méthodes

| Nom | La description |
| --- | --- |
| [Add](../../aspose.cells/hyperlinkcollection/add#add_1)(string, int, int, string) | Ajoute un lien hypertexte vers une cellule spécifiée ou une plage de cellules. |
| [Add](../../aspose.cells/hyperlinkcollection/add#add)(int, int, int, int, string) | Ajoute un lien hypertexte vers une cellule spécifiée ou une plage de cellules. |
| [Add](../../aspose.cells/hyperlinkcollection/add#add_2)(string, string, string, string, string) | Ajoute un lien hypertexte vers une cellule spécifiée ou une plage de cellules. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Hyperlink) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Hyperlink, IComparer&lt;Hyperlink&gt;) |  |
| [Clear](../../aspose.cells/hyperlinkcollection/clear#clear)() | Efface tous les hyperliens. (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Hyperlink) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Hyperlink[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Hyperlink[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Hyperlink[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Hyperlink&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Hyperlink&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Hyperlink&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Hyperlink&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Hyperlink) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Hyperlink, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Hyperlink, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Hyperlink) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Hyperlink, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Hyperlink, int, int) |  |
| [RemoveAt](../../aspose.cells/hyperlinkcollection/removeat#removeat)(int) | Supprimer le lien hypertexte à l'index spécifié. (2 methods) |

### Exemples

```csharp


[C#]

//Instanciation d'un objet Workbook
Workbook workbook = new Workbook();

//Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Worksheet worksheet = workbook.Worksheets[0];

//Obtenir la collection de liens hypertexte
HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

//Ajout d'un lien hypertexte vers une URL dans la cellule "A1"
hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

//Enregistrement du fichier Excel
workbook.Save("book1.xls");

[VB.NET]

'Instanciation d'un objet Workbook
Dim workbook As Workbook = New Workbook()

'Obtenir la référence de la feuille de calcul nouvellement ajoutée en passant son index de feuille
Dim worksheet As Worksheet = workbook.Worksheets(0)

'Obtenir la collection de liens hypertexte
Dim hyperlinks As HyperlinkCollection = worksheet.Hyperlinks

'Adding a hyperlink to a URL at "A1" cell
hyperlinks.Add("A1", 1, 1, "http://www.aspose.com")

'Enregistrement du fichier Excel
workbook.Save("book1.xls")
```

### Voir également

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Hyperlink](../hyperlink)
* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
