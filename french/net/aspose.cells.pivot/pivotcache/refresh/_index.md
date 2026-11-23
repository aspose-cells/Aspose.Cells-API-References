---
title: "PivotCache.Refresh"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotCache. Rafraîchit les données de la source de données et calcule les données pour la vue de tous les tableaux croisés dynamiques dont la source de données est ce cache de pivot."
type: docs
url: /fr/net/aspose.cells.pivot/pivotcache/refresh/
---
## Refresh(PivotTableRefreshOption) {#refresh_1}

Actualise les données depuis la source de données et calcule les données pour la vue de tous les tableaux croisés dynamiques dont la source de données est ce cache de tableau croisé dynamique.

```csharp
public PivotRefreshState Refresh(PivotTableRefreshOption option)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | Les options pour actualiser la source de données du tableau croisé dynamique. |

### Remarques

Il est préférable que vous puissiez simplement appeler [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) pour actualiser tous les tableaux croisés dynamiques et graphiques du fichier.

### Voir aussi

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Refresh() {#refresh}

Actualise les données depuis la source de données et calcule les données pour la vue de tous les tableaux croisés dynamiques dont la source de données est ce cache de tableau croisé dynamique.

```csharp
public PivotRefreshState Refresh()
```

### Remarques

Si table1 et table2 utilisent ce cache, les deux tables seront calculées. Il est préférable que vous puissiez simplement appeler [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) pour actualiser tous les tableaux croisés dynamiques et graphiques du fichier.

### Voir aussi

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotCache](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


