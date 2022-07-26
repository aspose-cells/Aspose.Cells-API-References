---
title: Add
second_title: Référence de l'API Aspose.Cells pour .NET
description: Ajoute un nouveau cache de tableau croisé dynamique à une collection PivotCaches.
type: docs
weight: 20
url: /fr/net/aspose.cells.pivot/pivottablecollection/add/
---
## Add(string, string, string) {#add_4}

Ajoute un nouveau cache de tableau croisé dynamique à une collection PivotCaches.

```csharp
public int Add(string sourceData, string destCellName, string tableName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sourceData | String | Les données du nouveau cache de tableau croisé dynamique. |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | String | Nom du nouveau rapport de tableau croisé dynamique. |

### Return_Value

Le nouvel index de cache ajouté.

### Voir également

* class [PivotTableCollection](../../pivottablecollection)
* espace de noms [Aspose.Cells.Pivot](../../pivottablecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(string, string, string, bool) {#add_5}

Ajoute un nouveau cache de tableau croisé dynamique à une collection PivotCaches.

```csharp
public int Add(string sourceData, string destCellName, string tableName, bool useSameSource)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sourceData | String | Les données du nouveau cache de tableau croisé dynamique. |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | String | Nom du nouveau rapport de tableau croisé dynamique. |
| useSameSource | Boolean | Indique si la même source de données est utilisée lorsqu'un autre tableau croisé dynamique existant a utilisé cette source de données. Si la propriété est vraie, cela économisera de la mémoire. |

### Return_Value

Le nouvel index de cache ajouté.

### Voir également

* class [PivotTableCollection](../../pivottablecollection)
* espace de noms [Aspose.Cells.Pivot](../../pivottablecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_2}

Ajoute un nouveau cache de tableau croisé dynamique à une collection PivotCaches.

```csharp
public int Add(string sourceData, int row, int column, string tableName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sourceData | String | La plage de cellules de données pour le nouveau tableau croisé dynamique.Exemple : Sheet1!A1:C8 |
| row | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | String | Nom du nouveau rapport de tableau croisé dynamique. |

### Return_Value

Le nouvel index de cache ajouté.

### Voir également

* class [PivotTableCollection](../../pivottablecollection)
* espace de noms [Aspose.Cells.Pivot](../../pivottablecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(string, int, int, string, bool) {#add_3}

Ajoute un nouveau cache de tableau croisé dynamique à une collection PivotCaches.

```csharp
public int Add(string sourceData, int row, int column, string tableName, bool useSameSource)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sourceData | String | La plage de cellules de données pour le nouveau tableau croisé dynamique.Exemple : Sheet1!A1:C8 |
| row | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | String | Nom du nouveau rapport de tableau croisé dynamique. |
| useSameSource | Boolean | Indique si la même source de données est utilisée lorsqu'un autre tableau croisé dynamique existant a utilisé cette source de données. Si la propriété est vraie, cela économisera de la mémoire. |

### Return_Value

Le nouvel index de cache ajouté.

### Voir également

* class [PivotTableCollection](../../pivottablecollection)
* espace de noms [Aspose.Cells.Pivot](../../pivottablecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(PivotTable, string, string) {#add_1}

Ajoute un nouvel objet de tableau croisé dynamique à la collection à partir d'un autre tableau croisé dynamique.

```csharp
public int Add(PivotTable pivotTable, string destCellName, string tableName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pivotTable | PivotTable | Le tableau croisé dynamique source. |
| destCellName | String | La cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | String | Nom du nouveau rapport de tableau croisé dynamique. |

### Return_Value

Le nouvel index de tableau croisé dynamique ajouté.

### Voir également

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* espace de noms [Aspose.Cells.Pivot](../../pivottablecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(PivotTable, int, int, string) {#add}

Ajoute un nouvel objet de tableau croisé dynamique à la collection à partir d'un autre tableau croisé dynamique.

```csharp
public int Add(PivotTable pivotTable, int row, int column, string tableName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pivotTable | PivotTable | Le tableau croisé dynamique source. |
| row | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | String | Nom du nouveau rapport de tableau croisé dynamique. |

### Return_Value

Le nouvel index de tableau croisé dynamique ajouté.

### Voir également

* class [PivotTable](../../pivottable)
* class [PivotTableCollection](../../pivottablecollection)
* espace de noms [Aspose.Cells.Pivot](../../pivottablecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, string, string) {#add_7}

Ajoute un nouvel objet de tableau croisé dynamique à la collection avec plusieurs plages de consolidation comme source de données.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, 
    string destCellName, string tableName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sourceData | String[] | Les plages de consolidation multiples, telles que {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Si créer automatiquement un champ de page unique. Si vrai, le paramètre suivant pageFields sera ignoré. |
| pageFields | PivotPageFields | Les éléments de champ de la page pivot. |
| destCellName | String | destCellName Le nom du nouveau rapport de tableau croisé dynamique. |
| tableName | String | le nom du nouveau rapport de tableau croisé dynamique. |

### Return_Value

Le nouvel index de tableau croisé dynamique ajouté.

### Voir également

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* espace de noms [Aspose.Cells.Pivot](../../pivottablecollection)
* Assemblée [Aspose.Cells](../../../)

---

## Add(string[], bool, PivotPageFields, int, int, string) {#add_6}

Ajoute un nouvel objet de tableau croisé dynamique à la collection avec plusieurs plages de consolidation comme source de données.

```csharp
public int Add(string[] sourceData, bool isAutoPage, PivotPageFields pageFields, int row, 
    int column, string tableName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sourceData | String[] | Les plages de consolidation multiples, telles que {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | Boolean | Si créer automatiquement un champ de page unique. Si vrai, le paramètre suivant pageFields sera ignoré |
| pageFields | PivotPageFields | Les éléments de champ de la page pivot. |
| row | Int32 | Index de ligne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| column | Int32 | Index de colonne de la cellule dans le coin supérieur gauche de la plage de destination du rapport de tableau croisé dynamique. |
| tableName | String | Nom du nouveau rapport de tableau croisé dynamique. |

### Return_Value

Le nouvel index de tableau croisé dynamique ajouté.

### Voir également

* class [PivotPageFields](../../pivotpagefields)
* class [PivotTableCollection](../../pivottablecollection)
* espace de noms [Aspose.Cells.Pivot](../../pivottablecollection)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
