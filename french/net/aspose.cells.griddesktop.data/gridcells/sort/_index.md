---
title: "GridCells.Sort"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridCells. Trie les données de façon ascendante/descendante de haut en bas dans une plage d'une feuille de calcul selon l'index de colonne spécifié. Trie les données de façon ascendante/descendante de gauche à droite dans une plage d'une feuille de calcul selon l'index de ligne spécifié."
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridcells/sort/
---
## Sort(int, int, int, int, int, bool, bool, bool) {#sort}

Trie les données de haut en bas dans une plage d'une feuille de calcul selon l'index de colonne spécifié. Trie les données de gauche à droite dans une plage d'une feuille de calcul selon l'index de ligne spécifié.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, bool isAsending, 
    bool isCaseSensitive, bool islefttoright)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Le numéro de ligne de la première cellule à trier. |
| startColumn | Int32 | Le numéro de colonne de la première cellule à trier. |
| lignes | Int32 | Nombre de lignes à importer. |
| colonnes | Int32 | Nombre de colonnes à importer. |
| indice | Int32 | Le numéro d'index de colonne qui spécifie la colonne de tri. Si l'Orientation est de haut en bas, il représente l'index de colonne qui spécifie la colonne de tri. Si l'Orientation est de gauche à droite, il représente l'index de ligne qui spécifie la ligne de tri. |
| isAsending | Boolean | indique si l'ordre de tri est ascendant. |
| isCaseSensitive | Boolean | indique si le tri est sensible à la casse. |
| islefttoright | Boolean | indique si l'orientation du tri est de gauche à droite |

### Exemples

```csharp

 [C#]

 GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### Voir aussi

* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Sort(int, int, int, int, int[], SortOrder[], SortOrientation, bool) {#sort_1}

Trie les données de la zone.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| Paramètre | Description |
| --- | --- |
| cellules | Les cellules contiennent la zone de données. |
| startRow | La ligne de départ de la zone. |
| startColumn | La colonne de départ de la zone. |
| lignes | le nombre total de lignes. |
| colonnes | Le nombre total de colonnes. |
| index | Le tableau d'index de colonnes triées |
| ordres | Le tableau d'ordres triés |
| orientation | l'orientation du tri : de gauche à droite ou de haut en bas. |
| isCaseSensitive | indique si la comparaison de chaînes est sensible à la casse.. |

### Voir aussi

* enum [SortOrder](../../../aspose.cells.griddesktop/sortorder/)
* enum [SortOrientation](../../../aspose.cells.griddesktop/sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


