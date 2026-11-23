---
title: "GridCells.Sort"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridCells. Trie les données de façon ascendante/descendante de haut en bas dans une plage d'une feuille de calcul selon l'index de colonne spécifié. Trie les données de façon ascendante/descendante de gauche à droite dans une plage d'une feuille de calcul selon l'index de ligne spécifié."
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridcells/sort/
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
 GridWeb GridWeb1 = new GridWeb();
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,3,true,true,false);

 [VB]

 GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3,true,true,false)

```

### Voir aussi

* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_1}

Trie les données de haut en bas dans une plage d'une feuille de calcul selon l'index de colonne spécifié. Trie les données de gauche à droite dans une plage d'une feuille de calcul selon l'index de ligne spécifié.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes, 
    SortByOrder[] orders, SortOrientation orientation, bool isCaseSensitive)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Le numéro de ligne de la première cellule à trier. |
| startColumn | Int32 | Le numéro de colonne de la première cellule à trier. |
| lignes | Int32 | Nombre de lignes à importer. |
| colonnes | Int32 | Nombre de colonnes à importer. |
| index | Int32[] | Le tableau d'indices de colonne qui spécifie la colonne de tri. Si l'Orientation est de haut en bas, il représente l'indice de colonne qui spécifie la colonne de tri. Si l'Orientation est de gauche à droite, il représente l'indice de ligne qui spécifie la ligne de tri. |
| ordres | SortByOrder[] | le tableau d'ordre de tri. |
| orientation | SortOrientation | orientation de tri |
| isCaseSensitive | Boolean | indique si le tri est sensible à la casse. |

### Exemples

```csharp

 [C#]
 GridWeb GridWeb1=new GridWeb();
 int[] ids={0,1};
 SortByOrder[] sorder={SortByOrder.Ascending,SortByOrder.Descending};
 GridWeb1.WorkSheets[0].Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false);

 [VB]

 GridWeb1.WorkSheets(0).Cells.Sort(1,0,25,6,ids,sorder,SortOrientation.SortTopToBottom,false)

```

### Voir aussi

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [GridCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


