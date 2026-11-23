---
title: "Worksheet.AddCustomFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Ajoute un filtre personnalisé pour la plage de lignes spécifiée du numéro de ligne de début à la ligne de fin"
type: docs
url: /fr/net/aspose.cells.griddesktop/worksheet/addcustomfilter/
---
## AddCustomFilter(int, int, object[], GridFilterOperatorType[]) {#addcustomfilter}

Ajoute un filtre personnalisé pour la plage de lignes spécifiée du début à la fin.

```csharp
public void AddCustomFilter(int startrow, int startcolumn, object[] critiras, 
    GridFilterOperatorType[] filterOperatorTypes)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| startrow | Int32 | Le startrow de la plage de filtre |
| startcolumn | Int32 | Le startcolumn de la plage de filtre |
| critiras | Object[] | Le tableau critira pour les colonnes, chacun s'applique à chaque colonne |
| filterOperatorTypes | GridFilterOperatorType[] | Le tableau des types d'opération de filtre pour les colonnes, chacun s'applique à chaque colonne |

### Voir aussi

* enum [GridFilterOperatorType](../../../aspose.cells.griddesktop.data/gridfilteroperatortype/)
* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## AddCustomFilter(int, string) {#addcustomfilter_1}

Ajoute un filtre personnalisé pour la ligne spécifiée.

```csharp
public void AddCustomFilter(int row, string critira)
```

### Remarques

La chaîne de critères de filtre. Notez que nous utilisons , et ; comme caractères de séparation, donc la valeur de la cellule ne doit pas contenir ces caractères de séparation. Ci-dessous les exemples de chaînes de critères : //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

### Voir aussi

* class [Worksheet](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


