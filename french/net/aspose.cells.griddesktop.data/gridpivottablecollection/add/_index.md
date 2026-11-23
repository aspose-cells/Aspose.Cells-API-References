---
title: "GridPivotTableCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GridPivotTableCollection. Ajoute un nouveau cache de tableau croisé dynamique à une collection PivotCaches"
type: docs
url: /fr/net/aspose.cells.griddesktop.data/gridpivottablecollection/add/
---
## Add(string, string, string) {#add_3}

Ajoute un nouveau cache PivotTable à une collection PivotCaches.

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceData | String | La plage de cellules de données pour le nouveau tableau croisé dynamique. Exemple : Sheet1!A1:C8 |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | String | Le nom du nouveau rapport de tableau croisé dynamique. |

### Valeur de retour

L'index du nouveau cache ajouté.

### Voir aussi

* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(Worksheet, GridCellArea, string, string) {#add}

Ajoute un nouveau cache PivotTable à une collection PivotCaches.

```csharp
public int Add(Worksheet sourceSheet, GridCellArea sourceArea, string destCellName, 
    string tableName)
```

| Paramètre | Description |
| --- | --- |
| sourceSheet | La feuille de calcul source. |
| sourceArea | La zone dans la feuille de calcul source. |
| destRow | La ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| destCol | La colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | Le nom du nouveau rapport de tableau croisé dynamique. |

### Valeur de retour

L'index du nouveau cache ajouté.

### Voir aussi

* class [Worksheet](../../../aspose.cells.griddesktop/worksheet/)
* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, GridCellArea, int, int, string) {#add_1}

Ajoute un nouveau cache PivotTable à une collection PivotCaches.

```csharp
public int Add(string worksheetname, GridCellArea sourceArea, int destRow, int destCol, 
    string tableName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| worksheetname | String | Le nom de la feuille de calcul source. |
| sourceArea | GridCellArea | La zone dans la feuille de calcul source. |
| destRow | Int32 | La ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| destCol | Int32 | La colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | String | Le nom du nouveau rapport de tableau croisé dynamique. |

### Valeur de retour

L'index du nouveau cache ajouté.

### Voir aussi

* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(string, GridCellArea, string, string) {#add_2}

Ajoute un nouveau cache PivotTable à une collection PivotCaches.

```csharp
public int Add(string worksheetname, GridCellArea sourceArea, string destCellName, string tableName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| worksheetname | String | Le nom de la feuille de calcul source. |
| sourceArea | GridCellArea | La zone dans la feuille de calcul source. |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | String | Le nom du nouveau rapport de tableau croisé dynamique. |

### Valeur de retour

L'index du nouveau cache ajouté.

### Voir aussi

* class [GridCellArea](../../gridcellarea/)
* class [GridPivotTableCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


