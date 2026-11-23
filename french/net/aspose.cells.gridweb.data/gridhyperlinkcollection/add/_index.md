---
title: "GridHyperlinkCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridHyperlinkCollection. Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridhyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | Première ligne de la plage d'hyperliens. |
| firstColumn | Int32 | Première colonne de la plage d'hyperliens. |
| totalRows | Int32 | Nombre de lignes dans cette plage d'hyperliens. |
| totalColumns | Int32 | Nombre de colonnes de cette plage d'hyperliens. |
| address | String | Adresse de l'hyperlien. |

### Valeur de retour

[`GridHyperlink`](../../gridhyperlink/) object index.

### Voir aussi

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(string, int, int, string) {#add_1}

Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Nom de la cellule. |
| totalRows | Int32 | Nombre de lignes dans cette plage d'hyperliens. |
| totalColumns | Int32 | Nombre de colonnes de cette plage d'hyperliens. |
| address | String | Adresse de l'hyperlien. |

### Valeur de retour

[`GridHyperlink`](../../gridhyperlink/) object index.

### Voir aussi

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(string, string) {#add_2}

Ajoute un hyperlien à une cellule spécifiée.

```csharp
public int Add(string cellName, string address)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| cellName | String | Nom de la cellule. |
| address | String | Adresse de l'hyperlien. |

### Valeur de retour

[`GridHyperlink`](../../gridhyperlink/) object index.

### Voir aussi

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(string, string, string, string, string) {#add_3}

Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startCellName | String | La cellule en haut à gauche de la plage. |
| endCellName | String | La cellule en bas à droite de la plage. |
| address | String | Adresse de l'hyperlien. |
| textToDisplay | String | Le texte à afficher pour l'hyperlien spécifié. |
| screenTip | String | Le texte screenTip pour le lien hypertexte spécifié. |

### Valeur de retour

[`GridHyperlink`](../../gridhyperlink/) object index.

### Voir aussi

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


