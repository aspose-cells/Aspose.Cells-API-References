---
title: "WebCells.Sort"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WebCells method. Trie les données de haut en bas dans une plage d'une WebWorksheet selon l'index de colonne spécifié"
type: docs
url: /fr/net/aspose.cells.gridweb.data/webcells/sort/
---
## Sort(int, int, int, int, int) {#sort}

Trie les données en ordre ascendant de haut en bas dans une plage d'un WebWorksheet selon l'index de colonne spécifié.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Le numéro de ligne de la première cellule à trier. |
| startColumn | Int32 | Le numéro de colonne de la première cellule à trier. |
| lignes | Int32 | Nombre de lignes à importer. |
| colonnes | Int32 | Nombre de colonnes à importer. |
| indice | Int32 | L'index de colonne qui spécifie la colonne de tri. |

### Exemples

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,3);

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,3)

```

### Voir aussi

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int, SortByOrder, SortOrientation, bool) {#sort_1}

Trie les données en ordre ascendant de haut en bas dans une plage d'un WebWorksheet selon l'index de colonne spécifié.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int index, 
    SortByOrder sortOrder, SortOrientation sortOrientation, bool isCaseSensitive)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Le numéro de ligne de la première cellule à trier. |
| startColumn | Int32 | Le numéro de colonne de la première cellule à trier. |
| lignes | Int32 | Nombre de lignes à importer. |
| colonnes | Int32 | Nombre de colonnes à importer. |
| indice | Int32 | L'index de colonne (ou de ligne) qui spécifie la colonne (ou la ligne) de tri. Si l'orientation du tri est de haut en bas, l'index représente l'index de colonne. Si l'orientation du tri est de gauche à droite, l'index représente l'index de ligne. |
| ordre | SortByOrder | L'ordre de tri : Ascendant ou Descendant |
| orientation | SortOrientation | L'orientation du tri : de haut en bas ou de gauche à droite. |
| isCaseSensitive | Boolean | Indique si les données de tri sont sensibles à la casse lorsque les données sont une chaîne. |

### Exemples

```csharp

[C#]

GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,true)

[VB]

GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,3,SortOrder.Ascending,SortOrientation.SortLeftToRight,True)

```

### Voir aussi

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[]) {#sort_2}

Trie les données en ordre ascendant de haut en bas dans une plage d'un WebWorksheet selon certains champs spécifiés par un tableau d'index de colonnes.

```csharp
public void Sort(int startRow, int startColumn, int rows, int columns, int[] indexes)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Le numéro de ligne de la première cellule à trier. |
| startColumn | Int32 | Le numéro de colonne de la première cellule à trier. |
| lignes | Int32 | Nombre de lignes à importer. |
| colonnes | Int32 | Nombre de colonnes à importer. |
| index | Int32[] | Le tableau des index de colonnes qui spécifie les données triées. |

### Exemples

```csharp

[C#]

int[] indexes = new int[3];
indexes[0] = 0;
indexes[1] = 2;
indexes[2] = 3;
GridWeb1.WebWorksheets[0].Cells.Sort(1,0,25,6,indexes);

[VB]

Dim indexes() As Integer =  New Integer(3) {} 
indexes(0) = 0
indexes(1) = 2
indexes(2) = 3
GridWeb1.WebWorksheets(0).Cells.Sort(1,0,25,6,indexes)

```

### Voir aussi

* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Sort(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) {#sort_3}

Trie les données en ordre ascendant dans une plage d'un WebWorksheet selon certains champs spécifiés par un tableau d'index.

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
| index | Int32[] | L'index de colonne (ou de ligne) qui spécifie la colonne (ou la ligne) de tri. Si l'orientation du tri est de haut en bas, l'index représente l'index de colonne. Si l'orientation du tri est de gauche à droite, l'index représente l'index de ligne. |
| ordres | SortByOrder[] | L'ordre de tri : Ascendant ou Descendant |
| orientation | SortOrientation | L'orientation du tri : de haut en bas ou de gauche à droite. |
| isCaseSensitive | Boolean | Indique si le tri est sensible à la casse. |

### Remarques

Si vous utilisez cette méthode pour trier un bloc de données, assurez-vous que la longueur du paramètre indexes est égale à la longueur du paramètre orders.

### Exemples

```csharp

```

[C#] int[] indexes = new int[3]; indexes[0] = 0; indexes[1] = 1; indexes[2] = 3; SortOrder[] orders = new SortOrder[3]; orders[0] = SortOrder.Ascending; orders[1] = SortOrder.Descending; orders[2] = SortOrder.Descending; GridWeb1.WebWorksheets[0].Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,false); [VB] Dim indexes() As Integer = New Integer(3) {} indexes(0) = 0 indexes(1) = 1 indexes(2) = 3 Dim orders() As SortOrder = New SortOrder(3) {} orders(0) = SortOrder.Ascending orders(1) = SortOrder.Descending orders(2) = SortOrder.Descending GridWeb1.WebWorksheets(0).Cells.Sort(0,1,4,14,indexes,orders,SortOrientation.SortLeftToRight,False)

### Voir aussi

* enum [SortByOrder](../../sortbyorder/)
* enum [SortOrientation](../../sortorientation/)
* class [WebCells](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


