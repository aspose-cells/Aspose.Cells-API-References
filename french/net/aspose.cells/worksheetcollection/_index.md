---
title: WorksheetCollection
second_title: Référence de l'API Aspose.Cells pour .NET
description: Encapsule une collection deWorksheet./worksheet objets.
type: docs
weight: 6520
url: /fr/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Encapsule une collection de[`Worksheet`](../worksheet) objets.

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Propriétés

| Nom | La description |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex) { get; set; } | Représente l'index de la feuille de calcul active lorsque la feuille de calcul est ouverte. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname) { get; set; } | Représente le nom de la feuille de calcul active lorsque la feuille de calcul est ouverte. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties) { get; } | Renvoie un[`DocumentProperty`](../../aspose.cells.properties/documentproperty)collection qui représente toutes les propriétés de document intégrées de la feuille de calcul. |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties) { get; } | Renvoie un[`DocumentProperty`](../../aspose.cells.properties/documentproperty) collection qui représente toutes les propriétés de document personnalisées de la feuille de calcul. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs) { get; } | Obtient les enregistrements principaux de formatage différentiel. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks) { get; } | Représente les liens externes dans un classeur. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections) { get; set; } | Indique si toutes les connexions sont actualisées à l'ouverture du fichier dans MS Excel. |
| [Item](../../aspose.cells/worksheetcollection/item) { get; } | Obtient le[`Worksheet`](../worksheet) élément à l'index spécifié. (2 indexers) |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names) { get; } | Obtient la collection de tous les objets Name de la feuille de calcul. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize) { get; set; } | Obtient et définit la taille affichée lorsque le fichier Workbook est utilisé comme objet Ole. |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs) { get; } | Représente les journaux de révision. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles) { get; } | Obtient[`TableStyles`](./tablestyles) objet. |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors) { get; } | Obtient la liste des auteurs de commentaires thématiques. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions) { get; } | Obtient la liste des volets de tâches. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes) { get; } | Obtient la liste des volets de tâches. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps) { get; set; } | Obtient et définit les mappages XML dans le classeur. |

## Méthodes

| Nom | La description |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add#add_1)() | Ajoute une feuille de calcul à la collection. |
| [Add](../../aspose.cells/worksheetcollection/add#add_2)(SheetType) | Ajoute une feuille de calcul à la collection. |
| [Add](../../aspose.cells/worksheetcollection/add#add)(string) | Ajoute une feuille de calcul à la collection. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy)(int) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy#addcopy_1)(string) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear#clear)() | Effacer toutes les feuilles de calcul. (2 methods) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables)() | Efface les tableaux croisés dynamiques de la feuille de calcul. |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange)(string, int) | Crée un[`Range`](../range) objet à partir d'une adresse de la plage. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange)(string, int) | Crée un[`Range`](../range) objet à partir d'une adresse de la plage. |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges)() | Obtient toutes les plages nommées prédéfinies dans la feuille de calcul. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables)() | Obtient toutes les plages nommées prédéfinies dans la feuille de calcul. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname)(string) | Obtient l'objet Range par nom prédéfini. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname#getrangebyname_1)(string, int, bool) | Obtient[`Range`](../range) par nom prédéfini ou nom de table |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename)(string) | Obtient la feuille de calcul par le nom de code. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert)(int, SheetType) | Insérer une feuille de calcul. |
| [Insert](../../aspose.cells/worksheetcollection/insert#insert_1)(int, SheetType, string) | Insérer une feuille de calcul. |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Worksheet, int, int) |  |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables)() | Actualise tous les tableaux croisés dynamiques dans la WorksheetCollection. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction_1)(int, string) | Ajoute une fonction complémentaire dans le classeur |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction#registeraddinfunction)(string, string, bool) | Ajoute une fonction complémentaire dans le classeur |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat)(int) | Supprime l'élément à un index spécifié. (2 methods) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat#removeat_2)(string) | Supprime l'élément à un nom spécifié. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize)(int, int, int, int) | Définit la taille affichée lorsque le fichier Workbook est utilisé comme objet Ole. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames)() | Trie les noms définis. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet)(int, int) | Échange les deux feuilles. |

### Exemples

```csharp
[C#]

Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;

//Ajouter une feuille de calcul
sheets.Add();

//Changer le nom d'une feuille de calcul
sheets[0].Name = "First Sheet";

// Définit la feuille active sur la deuxième feuille de calcul
sheets.ActiveSheetIndex = 1;

	
[Visual Basic]

Dim excel as Workbook = new Workbook()

Dim sheets as WorksheetCollection = excel.Worksheets

'Ajouter une feuille de calcul
sheets.Add()

'Changer le nom d'une feuille de calcul
sheets(0).Name = "First Sheet"

'Définir la feuille active sur la deuxième feuille de calcul
sheets.ActiveSheetIndex = 1
```

### Voir également

* class [CollectionBase&lt;T&gt;](../collectionbase-1)
* class [Worksheet](../worksheet)
* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
