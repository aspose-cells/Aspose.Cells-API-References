---
title: "Classe WorksheetCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.WorksheetCollection. Encapsule une collection d'objets Worksheet"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/
---
## WorksheetCollection class

Encapsule une collection d'objets [`Worksheet`](../worksheet/).

```csharp
public class WorksheetCollection : CollectionBase<Worksheet>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [ActiveSheetIndex](../../aspose.cells/worksheetcollection/activesheetindex/) { get; set; } | Représente l'index de la feuille de calcul active lorsque le classeur est ouvert. |
| [ActiveSheetName](../../aspose.cells/worksheetcollection/activesheetname/) { get; set; } | Représente le nom de la feuille de calcul active lorsque le classeur est ouvert. |
| [BuiltInDocumentProperties](../../aspose.cells/worksheetcollection/builtindocumentproperties/) { get; } | Renvoie une collection [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) qui représente toutes les propriétés de document intégrées du classeur. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [CustomDocumentProperties](../../aspose.cells/worksheetcollection/customdocumentproperties/) { get; } | Renvoie une collection [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) qui représente toutes les propriétés de document personnalisées du classeur. |
| [Dxfs](../../aspose.cells/worksheetcollection/dxfs/) { get; } | Obtient les enregistrements de mise en forme différentielle maîtres. |
| [ExternalLinks](../../aspose.cells/worksheetcollection/externallinks/) { get; } | Représente les liens externes dans un classeur. |
| [IsRefreshAllConnections](../../aspose.cells/worksheetcollection/isrefreshallconnections/) { get; set; } | Indique si toutes les connexions doivent être actualisées à l'ouverture du fichier dans MS Excel. |
| [Item](../../aspose.cells/worksheetcollection/item/) { get; } | Obtient l'élément [`Worksheet`](../worksheet/) à l'index spécifié. (2 indexeurs) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Names](../../aspose.cells/worksheetcollection/names/) { get; } | Obtient la collection de tous les objets Name dans le classeur. |
| [OleSize](../../aspose.cells/worksheetcollection/olesize/) { get; set; } | Obtient et définit la taille affichée lorsque le fichier Workbook est utilisé comme objet Ole. |
| [PivotCaches](../../aspose.cells/worksheetcollection/pivotcaches/) { get; } | Obtient tous les [`PivotCache`](../../aspose.cells.pivot/pivotcache/). |
| [RevisionLogs](../../aspose.cells/worksheetcollection/revisionlogs/) { get; } | Représente les journaux de révision. |
| [SensitivityLabels](../../aspose.cells/worksheetcollection/sensitivitylabels/) { get; } | Représente toutes les étiquettes de sensibilité. |
| [TableStyles](../../aspose.cells/worksheetcollection/tablestyles/) { get; } | Obtient l'objet [`TableStyles`](./tablestyles/). |
| [ThreadedCommentAuthors](../../aspose.cells/worksheetcollection/threadedcommentauthors/) { get; } | Obtient la liste des auteurs de commentaires en fil. |
| [WebExtensions](../../aspose.cells/worksheetcollection/webextensions/) { get; } | Obtient la liste des volets de tâche. |
| [WebExtensionTaskPanes](../../aspose.cells/worksheetcollection/webextensiontaskpanes/) { get; } | Obtient la liste des volets de tâche. |
| [XmlMaps](../../aspose.cells/worksheetcollection/xmlmaps/) { get; set; } | Obtient et définit les cartes XML dans le classeur. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells/worksheetcollection/add/#add_1)() | Ajoute une feuille de calcul à la collection. |
| [Add](../../aspose.cells/worksheetcollection/add/#add_2)(SheetType) | Ajoute une feuille de calcul à la collection. |
| [Add](../../aspose.cells/worksheetcollection/add/#add)(string) | Ajoute une feuille de calcul à la collection. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy)(int) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_1)(string) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante. |
| [AddCopy](../../aspose.cells/worksheetcollection/addcopy/#addcopy_2)(Worksheet[], string[]) | Copier un groupe de feuilles de calcul. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Worksheet, IComparer&lt;Worksheet&gt;) |  |
| [Clear](../../aspose.cells/worksheetcollection/clear/#clear)() | Effacer toutes les feuilles de calcul. (2 méthodes) |
| [ClearPivottables](../../aspose.cells/worksheetcollection/clearpivottables/)() | Supprime les tableaux croisés dynamiques de la feuille de calcul. |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Worksheet) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Worksheet[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Worksheet[], int, int) |  |
| [CreateRange](../../aspose.cells/worksheetcollection/createrange/)(string, int) | Crée un objet [`Range`](../range/) à partir d'une adresse de la plage. |
| [CreateUnionRange](../../aspose.cells/worksheetcollection/createunionrange/)(string, int) | Crée un objet [`Range`](../range/) à partir d'une adresse de la plage. |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Worksheet&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Worksheet&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Worksheet&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Worksheet&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetNamedRanges](../../aspose.cells/worksheetcollection/getnamedranges/)() | Obtient toutes les plages nommées pré‑définies dans la feuille de calcul. |
| [GetNamedRangesAndTables](../../aspose.cells/worksheetcollection/getnamedrangesandtables/)() | Obtient toutes les plages nommées pré‑définies dans la feuille de calcul. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname)(string) | Obtient l'objet Range par son nom pré‑défini. |
| [GetRangeByName](../../aspose.cells/worksheetcollection/getrangebyname/#getrangebyname_1)(string, int, bool) | Obtient le [`Range`](../range/) par son nom pré‑défini ou le nom de la table |
| [GetSheetByCodeName](../../aspose.cells/worksheetcollection/getsheetbycodename/)(string) | Obtient la feuille de calcul par son nom de code. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Worksheet, int, int) |  |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert)(int, SheetType) | Insérer une feuille de calcul. |
| [Insert](../../aspose.cells/worksheetcollection/insert/#insert_1)(int, SheetType, string) | Insérer une feuille de calcul. |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Worksheet, int, int) |  |
| [RefreshAll](../../aspose.cells/worksheetcollection/refreshall/)() | (**Obsolete.**) Rafraîchir tous les tableaux croisés dynamiques et les graphiques avec la source du tableau croisé. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables_1)() | Rafraîchit tous les tableaux croisés dynamiques dans le fichier Excel. |
| [RefreshPivotTables](../../aspose.cells/worksheetcollection/refreshpivottables/#refreshpivottables)(PivotTableRefreshOption) | Rafraîchit tous les tableaux croisés dynamiques dans le fichier Excel. |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction_1)(int, string) | Ajoute la fonction d'add‑in dans le classeur |
| [RegisterAddInFunction](../../aspose.cells/worksheetcollection/registeraddinfunction/#registeraddinfunction)(string, string, bool) | Ajoute la fonction d'add‑in dans le classeur |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat)(int) | Supprime l'élément à un indice spécifié. (2 méthodes) |
| [RemoveAt](../../aspose.cells/worksheetcollection/removeat/#removeat_2)(string) | Supprime l'élément à un nom spécifié. |
| [SetOleSize](../../aspose.cells/worksheetcollection/setolesize/)(int, int, int, int) | Définit la taille affichée lorsque le fichier classeur est utilisé comme objet Ole. |
| [SortNames](../../aspose.cells/worksheetcollection/sortnames/)() | Trie les noms définis. |
| [SwapSheet](../../aspose.cells/worksheetcollection/swapsheet/)(int, int) | Échange les deux feuilles. |

### Exemples

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionDemo
    {
        public static void RunDemo()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;

            // Ajouter une nouvelle feuille de calcul à la collection
            int newSheetIndex = worksheets.Add(SheetType.Worksheet);
            Worksheet newSheet = worksheets[newSheetIndex];
            newSheet.Name = "NewSheet";

            // Accéder à une feuille de calcul existante par indice
            Worksheet firstSheet = worksheets[0];
            firstSheet.Name = "FirstSheet";

            // Accéder à une feuille de calcul existante par nom
            Worksheet retrievedSheet = worksheets["FirstSheet"];

            // Définir la feuille active
            worksheets.ActiveSheetIndex = newSheetIndex;

            // Définir le nom de la feuille active
            worksheets.ActiveSheetName = "NewSheet";

            // Rafraîchir tous les tableaux croisés dynamiques dans le classeur
            worksheets.RefreshAll();

            // Effacer tous les tableaux croisés dynamiques du classeur
            worksheets.ClearPivottables();

            // Enregistrez le classeur
            workbook.Save("WorksheetCollectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Worksheet](../worksheet/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


