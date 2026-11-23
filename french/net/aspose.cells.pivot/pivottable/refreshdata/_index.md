---
title: "PivotTable.RefreshData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Rafraîchit les données de sa source de données vers le cache de pivot"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/refreshdata/
---
## RefreshData() {#refreshdata}

Rafraîchit les données de sa source de données vers le cache de pivot.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData()
```

### Remarques

Nous collecterons les données de la source de données vers un cache de tableau croisé dynamique, puis calculerons les données du cache dans les cellules. Il est préférable que vous puissiez simplement appeler [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) pour actualiser et calculer tous les tableaux croisés dynamiques du fichier, au lieu de les actualiser un par un. NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode [`Refresh`](../../pivotcache/refresh/) et supprimer la méthode [`CalculateData`](../calculatedata/) car ce tableau croisé dynamique sera calculé lors de l'actualisation du [`PivotCache`](../pivotcache/). Cette méthode sera supprimée 12 mois plus tard, à compter de juin 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);
            
            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Ajouter des champs de ligne et de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Actualiser et calculer les données du tableau croisé dynamique
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Enregistrez le classeur
            workbook.Save("PivotTableRefreshDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## RefreshData(PivotTableRefreshOption) {#refreshdata_1}

Actualise les données et les paramètres du tableau croisé dynamique à partir de sa source de données avec des options.

```csharp
[Obsolete("Use PivotCache.Refresh() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotRefreshState RefreshData(PivotTableRefreshOption option)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | Les options pour actualiser la source de données du tableau croisé dynamique. |

### Remarques

Nous collecterons les données de la source de données vers un cache de tableau croisé dynamique, puis calculerons les données du cache dans les cellules. Il est préférable que vous puissiez simplement appeler [`RefreshAll`](../../../aspose.cells/workbook/refreshall/) pour actualiser et calculer tous les tableaux croisés dynamiques du fichier, au lieu de les actualiser un par un. NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode [`Refresh`](../../pivotcache/refresh/) et supprimer la méthode [`CalculateData`](../calculatedata/) car ce tableau croisé dynamique sera calculé lors de l'actualisation du [`PivotCache`](../pivotcache/). Cette méthode sera supprimée 12 mois plus tard, à compter de juin 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodRefreshDataWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            // Créer un classeur à partir du fichier Excel source
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accéder à la feuille de calcul contenant le tableau croisé dynamique
            Worksheet worksheet = workbook.Worksheets["PNL_AFS"];
            
            // Obtenir le premier tableau croisé dynamique dans la feuille de calcul
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Configurer les options d'actualisation
            PivotTableRefreshOption refreshOptions = new PivotTableRefreshOption();
            refreshOptions.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
            
            // Actualiser les données du tableau croisé dynamique avec les options spécifiées
            pivotTable.RefreshData(refreshOptions);
            pivotTable.CalculateData();
            
            // Enregistrer le classeur modifié
            workbook.Save("example_modified.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PivotRefreshState](../../pivotrefreshstate/)
* class [PivotTableRefreshOption](../../pivottablerefreshoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


