---
title: "Classe HtmlTableLoadOptionCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.HtmlTableLoadOptionCollection. Représente les options de tableau lors de l'importation du HTML"
type: docs
url: /fr/net/aspose.cells/htmltableloadoptioncollection/
---
## HtmlTableLoadOptionCollection class

Représente les options du tableau lors de l'importation de HTML.

```csharp
public class HtmlTableLoadOptionCollection : CollectionBase<HtmlTableLoadOption>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [HtmlTableLoadOptionCollection](htmltableloadoptioncollection/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/htmltableloadoptioncollection/item/) { get; } | Obtient l'élément [`HtmlTableLoadOption`](../htmltableloadoption/) à l'index spécifié. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [TableToListObject](../../aspose.cells/htmltableloadoptioncollection/tabletolistobject/) { get; set; } | Indique s'il faut générer des objets de liste à partir des tables importées. La valeur par défaut est false. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add)(HtmlTableLoadOption) | (**Obsolete.**) Ajoute un HtmlTableLoadOption à cette collection. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_1)(int) | Ajoutez un HtmlTableLoadOption à la liste. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_4)(string) | Ajoutez un HtmlTableLoadOption à la liste. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_2)(int, int) | Ajoutez un HtmlTableLoadOption à la liste. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_5)(string, int) | Ajoutez un HtmlTableLoadOption à la liste. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_3)(int, int, int) | Ajoutez un HtmlTableLoadOption à la liste. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_6)(string, int, int) | Ajoutez un HtmlTableLoadOption à la liste. |
| [AddTableLoadOption](../../aspose.cells/htmltableloadoptioncollection/addtableloadoption/)(HtmlTableLoadOption) | Ajoute un HtmlTableLoadOption à cette collection. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(HtmlTableLoadOption) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, HtmlTableLoadOption[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionCollectionDemo
    {
        public static void HtmlTableLoadOptionCollectionExample()
        {
            // Créez un nouveau classeur
            Workbook workbook = new Workbook();

            // Créez HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Accédez à l'instance HtmlTableLoadOptionCollection
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Définir la propriété TableToListObject
            tableLoadOptions.TableToListObject = true;

            // Ajouter une nouvelle HtmlTableLoadOption par indice de tableau
            int index1 = tableLoadOptions.Add(0);

            // Ajouter une nouvelle HtmlTableLoadOption par identifiant de tableau
            int index2 = tableLoadOptions.Add("tableId");

            // Ajouter une nouvelle HtmlTableLoadOption par indice de tableau et indice de feuille cible
            int index3 = tableLoadOptions.Add(1, 1);

            // Ajouter une nouvelle HtmlTableLoadOption par identifiant de tableau et indice de feuille cible
            int index4 = tableLoadOptions.Add("tableId2", 2);

            // Ajouter une nouvelle HtmlTableLoadOption par indice de tableau, indice de feuille cible et indice de feuille d'origine
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Ajouter une nouvelle HtmlTableLoadOption par identifiant de tableau, indice de feuille cible et indice de feuille d'origine
            int index6 = tableLoadOptions.Add("tableId3", 3, 1);

            // Accéder à la HtmlTableLoadOption à un indice spécifique
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Définir les propriétés de la HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = "tableId";
            option.Name = "TableName";
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Charger un fichier HTML dans le classeur en utilisant les options de chargement
            workbook = new Workbook("HtmlTableLoadOptionCollectionExample_original.html", loadOptions);

            // Enregistrez le classeur
            workbook.Save("HtmlTableLoadOptionCollectionExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [HtmlTableLoadOption](../htmltableloadoption/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


