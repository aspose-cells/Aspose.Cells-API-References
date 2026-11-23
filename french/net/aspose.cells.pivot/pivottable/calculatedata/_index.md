---
title: "PivotTable.CalculateData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Calcule les données du tableau croisé dynamique vers les cellules"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/calculatedata/
---
## CalculateData() {#calculatedata_1}

Calcule les données du pivottable dans les cellules.

```csharp
public void CalculateData()
```

### Remarques

Cette méthode ne calcule les données qu'avec les données mises en cache dans le [`PivotCache`](../pivotcache/). Ainsi, si vous souhaitez calculer avec la source de données la plus récente, veuillez utiliser la méthode [`Refresh`](../../pivotcache/refresh/) pour calculer. Si seuls les paramètres du tableau croisé dynamique sont modifiés, `CalculateData` suffit.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["B1"].PutValue("Sales");
            
            DateTime baseDate = new DateTime(2021, 11, 1);
            for (int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+2}"].PutValue(baseDate.AddDays(i));
                worksheet.Cells[$"B{i+2}"].PutValue(100 + i * 10);
            }

            // Créer un tableau croisé dynamique - corrigé en assurant des paramètres corrects
            int pivotIndex = worksheet.PivotTables.Add("A1:B16", "D3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Appliquer un filtre de date
            PivotField dateField = pivotTable.RowFields[0];
            dateField.FilterByDate(PivotFilterType.November, new DateTime(2021, 1, 1), new DateTime(2021, 12, 31));
            
            // Calculer les données du tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Enregistrez le classeur
            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## CalculateData(PivotTableCalculateOption) {#calculatedata}

Calcule le tableau croisé dynamique avec des options.

```csharp
public PivotTable[] CalculateData(PivotTableCalculateOption option)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| option | PivotTableCalculateOption | Les options pour calculer le tableau croisé dynamique |

### Valeur de retour

Renvoie tous les tableaux croisés dynamiques qui ont été calculés. Si [`RefreshData`](../../pivottablecalculateoption/refreshdata/) est vrai, tous les tableaux croisés dynamiques basés sur le même cache de pivot seront calculés ensemble.

### Remarques

Si [`RefreshData`](../../pivottablecalculateoption/refreshdata/) est vrai, cette méthode rafraîchira le cache de pivot à partir de la source de données, puis calculera tous les tableaux croisés dynamiques basés sur le même cache de pivot. Sinon, le calcul ne se fera qu'avec les données mises en cache dans le cache de pivot.

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateDataWithPivotTableCalculateOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Définissez les options de calcul
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                RefreshData = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calculer avec des options
            pivotTable.CalculateData(options);

            workbook.Save("PivotTableCalculateDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


