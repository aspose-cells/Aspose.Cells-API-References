---
title: "Classe NameCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.NameCollection. Représente une collection de tous les objets Name dans la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/namecollection/
---
## NameCollection class

Représente une collection de tous les objets [`Name`](../name/) dans la feuille de calcul.

```csharp
public class NameCollection : CollectionBase<Name>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/namecollection/item/) { get; } | Obtient l'élément [`Name`](../name/) à l'index spécifié. (2 indexeurs) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells/namecollection/add/)(string) | Définit un nouveau nom. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name, IComparer&lt;Name&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Name, IComparer&lt;Name&gt;) |  |
| [Clear](../../aspose.cells/namecollection/clear/#clear)() | Supprime tous les noms définis qui ne sont pas référencés par les formules et la source de données. Si le nom défini est référencé, nous ne faisons que définir Name.ReferTo à null et les masquer. (2 méthodes) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Name) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Name[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Name&gt;) |  |
| [Filter](../../aspose.cells/namecollection/filter/)(NameScopeType, int) | Obtient tous les noms définis par portée. |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Name&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int, int) |  |
| [Remove](../../aspose.cells/namecollection/remove/#remove)(string) | Supprimer le nom. |
| [Remove](../../aspose.cells/namecollection/remove/#remove_1)(string[]) | Supprimer un tableau de noms |
| [RemoveAt](../../aspose.cells/namecollection/removeat/#removeat)(int) | Supprimer le nom à l'index spécifique. (2 méthodes) |
| [RemoveDuplicateNames](../../aspose.cells/namecollection/removeduplicatenames/)() | Supprimer les noms définis en double |
| [Sort](../../aspose.cells/namecollection/sort/)() | Trie les noms définis. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionDemo
    {
        public static void NameCollectionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la collection de feuilles de calcul
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Accéder à la collection de noms
            NameCollection names = worksheets.Names;
            
            // Ajouter un nouveau nom à la collection
            int nameIndex = names.Add("MyNamedRange");
            Name name = names[nameIndex];
            
            // Définir la propriété "refers to" pour le nom
            name.RefersTo = "=Sheet1!$A$1:$A$10";
            
            // Accéder et modifier les propriétés du nom
            name.Comment = "This is a named range for demonstration.";
            name.IsVisible = true;
            
            // Ajouter un autre nom
            int anotherNameIndex = names.Add("AnotherNamedRange");
            Name anotherName = names[anotherNameIndex];
            anotherName.RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Supprimer un nom par texte
            names.Remove("AnotherNamedRange");
            
            // Supprimer un nom par index
            names.RemoveAt(nameIndex);
            
            // Effacer tous les noms
            names.Clear();
            
            // Enregistrez le classeur
            workbook.Save("NameCollectionExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Name](../name/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


