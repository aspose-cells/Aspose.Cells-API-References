---
title: Merge
second_title: Référence de l'API Aspose.Cells pour .NET
description: Fusionne une plage de cellules spécifiée en une seule cellule.
type: docs
weight: 1180
url: /fr/net/aspose.cells/cells/merge/
---
## Merge(int, int, int, int) {#merge}

Fusionne une plage de cellules spécifiée en une seule cellule.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| firstRow | Int32 | Première ligne de cette plage (base zéro) |
| firstColumn | Int32 | Première colonne de cette plage (base zéro) |
| totalRows | Int32 | Nombre de lignes (une base) |
| totalColumns | Int32 | Nombre de colonnes (une base) |

### Remarques

Référencez la cellule fusionnée via l'adresse de la cellule supérieure gauche de la plage.

### Voir également

* class [Cells](../../cells)
* espace de noms [Aspose.Cells](../../cells)
* Assemblée [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool) {#merge_1}

Fusionne une plage de cellules spécifiée en une seule cellule.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool mergeConflict)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| firstRow | Int32 | Première ligne de cette plage (base zéro) |
| firstColumn | Int32 | Première colonne de cette plage (base zéro) |
| totalRows | Int32 | Nombre de lignes (une base) |
| totalColumns | Int32 | Nombre de colonnes (une base) |
| mergeConflict | Boolean | Fusionner les plages fusionnées en conflit. |

### Remarques

Référencez la cellule fusionnée via l'adresse de la cellule supérieure gauche de la plage. Si mergeConflict est vrai et que la plage fusionnée est en conflit avec d'autres cellules fusionnées, les autres cellules fusionnées seront automatiquement supprimées.

### Voir également

* class [Cells](../../cells)
* espace de noms [Aspose.Cells](../../cells)
* Assemblée [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool, bool) {#merge_2}

Fusionne une plage de cellules spécifiée en une seule cellule.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool checkConflict, bool mergeConflict)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| firstRow | Int32 | Première ligne de cette plage (base zéro) |
| firstColumn | Int32 | Première colonne de cette plage (base zéro) |
| totalRows | Int32 | Nombre de lignes (une base) |
| totalColumns | Int32 | Nombre de colonnes (une base) |
| checkConflict | Boolean | Indique si cocher les cellules fusionnées croise d'autres cellules fusionnées |
| mergeConflict | Boolean | Fusionner les plages fusionnées en conflit. |

### Remarques

Référencez la cellule fusionnée via l'adresse de la cellule supérieure gauche de la plage. Si mergeConflict est vrai et que la plage fusionnée est en conflit avec d'autres cellules fusionnées, les autres cellules fusionnées seront automatiquement supprimées.

### Voir également

* class [Cells](../../cells)
* espace de noms [Aspose.Cells](../../cells)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
