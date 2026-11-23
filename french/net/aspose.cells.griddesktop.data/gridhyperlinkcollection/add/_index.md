---
title: "GridHyperlinkCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridHyperlinkCollection. Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules"
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridhyperlinkcollection/add/
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

Index de l'objet Hyperlink.

### Exemples

```csharp
[C#]

Worksheet worksheet = excel.Worksheets[0];
worksheet.Hyperlinks.Add("A4", 1, 1, "http://www.aspose.com");
worksheet.Hyperlinks.Add("A5", 1, 1, "c:\\book1.xls");

[Visual Basic]

Dim worksheet as Worksheet = excel.Worksheets(0)
worksheet.Hyperlinks.Add("A4", 1, 1, "http://www.aspose.com")
worksheet.Hyperlinks.Add("A5", 1, 1, "c:\\book1.xls")

```

### Voir aussi

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

Index de l'objet Hyperlink.

### Voir aussi

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

Index de l'objet Hyperlink.

### Voir aussi

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

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

Index de l'objet Hyperlink.

### Voir aussi

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, int, string) {#add_4}

Ajoute un hyperlien à une cellule spécifiée à l'index de ligne et de colonne.

```csharp
public void Add(int row, int col, string url)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| ligne | Int32 | Indice de ligne de la cellule. |
| col | Int32 | Indice de colonne de la cellule. |
| url | String | URL du lien hypertexte. |

### Voir aussi

* class [GridHyperlinkCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


