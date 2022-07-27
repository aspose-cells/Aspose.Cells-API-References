---
title: DataSorter
second_title: Référence de l'API Aspose.Cells pour .NET
description: Description sommaire de DataSorter.
type: docs
weight: 1300
url: /fr/net/aspose.cells/datasorter/
---
## DataSorter class

Description sommaire de DataSorter.

```csharp
public class DataSorter
```

## Propriétés

| Nom | La description |
| --- | --- |
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive) { get; set; } | Obtient et définit si la casse est sensible lors de la comparaison de chaîne. |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders) { get; set; } | Représente si la plage a des en-têtes. |
| [Key1](../../aspose.cells/datasorter/key1) { get; set; } | Représente le premier index de colonne trié (position absolue, la colonne A est 0, B est 1, ...). |
| [Key2](../../aspose.cells/datasorter/key2) { get; set; } | Représente l'index de la deuxième colonne triée (position absolue, la colonne A est 0, B est 1, ...). |
| [Key3](../../aspose.cells/datasorter/key3) { get; set; } | Représente le troisième index de colonne trié (position absolue, la colonne A est 0, B est 1, ...). |
| [Keys](../../aspose.cells/datasorter/keys) { get; } | Obtient la liste des clés du trieur de données. |
| [Order1](../../aspose.cells/datasorter/order1) { get; set; } | Représente l'ordre de tri de la première clé. |
| [Order2](../../aspose.cells/datasorter/order2) { get; set; } | Représente l'ordre de tri de la deuxième clé. |
| [Order3](../../aspose.cells/datasorter/order3) { get; set; } | Représente l'ordre de tri de la troisième clé. |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber) { get; set; } | Indique si trier tout ce qui ressemble à un nombre. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright) { get; set; } | True signifie que l'orientation du tri est de gauche à droite. False signifie que l'orientation du tri est de haut en bas. La valeur par défaut est false. |

## Méthodes

| Nom | La description |
| --- | --- |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_1)(int, SortOrder) | Ajoute un index de colonne trié et un ordre de tri. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_2)(int, SortOrder, string) | Ajoute un index de colonne trié et un ordre de tri avec une liste de tri personnalisée. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey_3)(int, SortOrder, string[]) | Ajoute un index de colonne trié et un ordre de tri avec une liste de tri personnalisée. |
| [AddKey](../../aspose.cells/datasorter/addkey#addkey)(int, SortOnType, SortOrder, object) | Ajoute un index de colonne trié et un ordre de tri avec une liste de tri personnalisée. |
| [Clear](../../aspose.cells/datasorter/clear)() | Effacer tous les paramètres. |
| [Sort](../../aspose.cells/datasorter/sort#sort)() | Trier les données dans la plage. |
| [Sort](../../aspose.cells/datasorter/sort#sort_1)(Cells, CellArea) | Trier les données de la zone. |
| [Sort](../../aspose.cells/datasorter/sort#sort_2)(Cells, int, int, int, int) | Trie les données de la zone. |

### Exemples

```csharp

[C#]

//Instancier un nouvel objet Workbook.
Workbook workbook = new Workbook("Book1.xls");
// Récupère l'objet de tri de données du classeur.
DataSorter sorter = workbook.DataSorter;
// Définit le premier ordre pour l'objet datasorter.
sorter.Order1 = Aspose.Cells.SortOrder.Descending;
// Définit la première clé.
sorter.Key1 = 0;
// Définit le deuxième ordre pour l'objet datasorter.
sorter.Order2 = Aspose.Cells.SortOrder.Ascending;
// Définit la deuxième clé.
sorter.Key2 = 1;
//Crée une zone de cellules (plage).
CellArea ca = new CellArea();
// Spécifiez l'index de la ligne de début.
ca.StartRow = 0;
// Spécifiez l'index de la colonne de départ.
ca.StartColumn = 0;
// Spécifiez l'index de la dernière ligne.
ca.EndRow = 13;
// Spécifiez le dernier index de colonne.
ca.EndColumn = 1;
//Trier les données dans la plage de données spécifiée (A1:B14)
sorter.Sort(workbook.Worksheets[0].Cells, ca);
// Enregistrez le fichier excel.
workbook.Save("outBook.xls");

[Visual Basic]

'Instanciez un nouvel objet Workbook.
Dim workbook As Workbook = New Workbook("Book1.xls")
'Obtenez l'objet de tri de données de classeur.
Dim sorter As DataSorter = workbook.DataSorter
'Définir le premier ordre pour l'objet datasorter
sorter.Order1 = Aspose.Cells.SortOrder.Descending
'Définissez la première clé.
sorter.Key1 = 0
'Définissez le deuxième ordre pour l'objet datasorter.
sorter.Order2 = Aspose.Cells.SortOrder.Ascending
'Définissez la deuxième clé.
sorter.Key2 = 1
'Créez une zone de cellules (plage).
Dim ca As CellArea = New CellArea
'Spécifiez l'index de la ligne de début.
ca.StartRow = 0
'Spécifiez l'index de la colonne de début.
ca.StartColumn = 0
'Spécifiez l'index de la dernière ligne.
ca.EndRow = 13
'Spécifiez le dernier index de colonne.
ca.EndColumn = 1
'Trier les données dans la plage de données spécifiée (A1:B14)
sorter.Sort(workbook.Worksheets(0).Cells, ca)
'Enregistrez le fichier excel.
workbook.Save("outBook.xls")

```

### Voir également

* espace de noms [Aspose.Cells](../../aspose.cells)
* Assemblée [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
