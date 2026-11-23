---
title: "Classe ColumnCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ColumnCollection. Collection des objets Column qui représentent les paramètres individuels des colonnes dans une feuille de calcul. L’objet Column ne représente que les paramètres tels que la largeur de colonne, les styles, etc., pour la colonne entière et n’a rien à voir avec le fait qu’il y ait ou non des données de cellules non vides dans la colonne correspondante. Et le Count de cette collection ne représente que le nombre d’objets Column qui ont été instanciés dans cette collection et n’a rien à voir avec le fait qu’il y ait ou non des données de cellules non vides dans la feuille de calcul."
type: docs
url: /fr/net/aspose.cells/columncollection/
---
## ColumnCollection class

Collection des objets [`Column`](../column/) qui représentent les colonnes (paramètre)s individuelles dans une feuille de calcul. L’objet Column ne représente que les paramètres tels que la largeur de colonne, les styles, etc., pour la colonne entière, et n’a rien à voir avec le fait qu’il existe ou non des cellules non vides (données) dans la colonne correspondante. Et le "Count" de cette collection ne représente que le nombre d’objets Column qui ont été instanciés dans cette collection, n’ayant rien à voir avec le fait qu’il existe ou non des cellules non vides (données) dans la feuille de calcul.

```csharp
public class ColumnCollection : CollectionBase<Column>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/columncollection/item/) { get; } | Obtient un objet [`Column`](../column/) par indice de colonne. L’objet Column de l’indice de colonne donné sera instancié s’il n’existe pas auparavant. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Column) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Column, IComparer&lt;Column&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Column, IComparer&lt;Column&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Column) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Column[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Column[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Column[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Column&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Column&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Column&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Column&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Column&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Column&gt;) |  |
| [GetByIndex](../../aspose.cells/columncollection/getbyindex/)(int) | (**Obsolète.**) Obtient l’objet colonne par l’indice. |
| [GetColumnByIndex](../../aspose.cells/columncollection/getcolumnbyindex/)(int) | Obtient l’objet [`Column`](../column/) par la position dans la liste. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Column, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Column, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnCollectionDemo
    {
        public static void ColumnCollectionExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();

            // Obtention de la référence de la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un nouveau Style au classeur
            Style style = workbook.CreateStyle();

            // Définition de la couleur d'arrière-plan en bleu
            style.ForegroundColor = Color.Blue;

            // Définition du motif d'arrière-plan
            style.Pattern = BackgroundType.Solid;

            // Nouveau drapeau de style
            StyleFlag styleFlag = new StyleFlag();

            // Définir tous les styles
            styleFlag.All = true;

            // Modifier la largeur par défaut des dix premières colonnes
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells.Columns[i].Width = 20;
            }

            // Obtenir la Column avec un formatage non par défaut
            ColumnCollection columns = worksheet.Cells.Columns;

            foreach (Column column in columns)
            {
                // Appliquer le Style aux dix premières Columns
                column.ApplyStyle(style, styleFlag);
            }

            // Enregistrement du fichier Excel
            workbook.Save("ColumnCollectionExample.xlsx");
            workbook.Save("ColumnCollectionExample.pdf");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Column](../column/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


