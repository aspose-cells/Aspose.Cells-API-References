---
title: "Classe DataSorter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.DataSorter. Description résumée pour DataSorter"
type: docs
url: /fr/net/aspose.cells/datasorter/
---
## DataSorter class

Description résumée pour DataSorter.

```csharp
public class DataSorter
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive/) { get; set; } | Obtient et définit si la comparaison de chaînes est sensible à la casse. |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders/) { get; set; } | Représente si la plage possède des en-têtes. |
| [Key1](../../aspose.cells/datasorter/key1/) { get; set; } | Représente l'index de la première colonne triée (position absolue, la colonne A vaut 0, B vaut 1, ...). |
| [Key2](../../aspose.cells/datasorter/key2/) { get; set; } | Représente l'index de la deuxième colonne triée (position absolue, la colonne A vaut 0, B vaut 1, ...). |
| [Key3](../../aspose.cells/datasorter/key3/) { get; set; } | Représente l'index de la troisième colonne triée (position absolue, la colonne A vaut 0, B vaut 1, ...). |
| [Keys](../../aspose.cells/datasorter/keys/) { get; } | Obtient la liste des clés du DataSorter. |
| [Order1](../../aspose.cells/datasorter/order1/) { get; set; } | Représente l'ordre de tri de la première clé. |
| [Order2](../../aspose.cells/datasorter/order2/) { get; set; } | Représente l'ordre de tri de la deuxième clé. |
| [Order3](../../aspose.cells/datasorter/order3/) { get; set; } | Représente l'ordre de tri de la troisième clé. |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber/) { get; set; } | Indique si le tri considère tout ce qui ressemble à un nombre. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright/) { get; set; } | Vrai signifie que l'orientation du tri est de gauche à droite. Faux signifie que l'orientation du tri est de haut en bas. La valeur par défaut est faux. |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddColorKey](../../aspose.cells/datasorter/addcolorkey/)(int, SortOnType, SortOrder, Color) | Ajoute une clé de tri de couleur. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_1)(int, SortOrder) | Ajoute l'index de colonne triée et l'ordre de tri. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_2)(int, SortOrder, string) | Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_3)(int, SortOrder, string[]) | Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey)(int, SortOnType, SortOrder, object) | Ajoute l'index de colonne triée et l'ordre de tri avec une liste de tri personnalisée. |
| [Clear](../../aspose.cells/datasorter/clear/)() | Efface tous les paramètres. |
| [Sort](../../aspose.cells/datasorter/sort/#sort)() | Trie les données dans la plage. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_1)(Cells, CellArea) | Trie les données de la zone. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_2)(Cells, int, int, int, int) | Trie les données de la zone. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterDemo
    {
        public static void DataSorterExample()
        {
            // Instancie un nouvel objet Workbook
            Workbook workbook = new Workbook("DataSorter_original.xlsx");

            // Obtenez l'objet DataSorter du classeur
            DataSorter sorter = workbook.DataSorter;

            // Définissez le premier ordre pour l'objet DataSorter
            sorter.Order1 = SortOrder.Descending;
            // Définissez la première clé
            sorter.Key1 = 0;

            // Définissez le deuxième ordre pour l'objet DataSorter
            sorter.Order2 = SortOrder.Ascending;
            // Définissez la deuxième clé
            sorter.Key2 = 1;

            // Créez une zone de cellules (plage)
            CellArea ca = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 13,
                EndColumn = 1
            };

            // Trie les données dans la plage de données spécifiée (A1:B14)
            sorter.Sort(workbook.Worksheets[0].Cells, ca);

            // Enregistrez le fichier Excel
            workbook.Save("DataSorterExample.xlsx");
            workbook.Save("DataSorterExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


