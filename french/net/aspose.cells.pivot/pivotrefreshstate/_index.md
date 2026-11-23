---
title: "Enum PivotRefreshState"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Pivot.PivotRefreshState enum. L'état pour actualiser les tableaux croisés dynamiques"
type: docs
url: /fr/net/aspose.cells.pivot/pivotrefreshstate/
---
## PivotRefreshState enumeration

L'état du rafraîchissement des tableaux croisés dynamiques.

```csharp
public enum PivotRefreshState
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Success | `0` | Rafraîchissement réussi |
| UnsupportedExternalDataSource | `1` | Échec du rafraîchissement car la source de données est externe. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotRefreshStateDemo
    {
        public static void Run()
        {
            // Créer un classeur avec un tableau croisé dynamique d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Démontrer PivotRefreshState
            PivotRefreshState refreshState = pivotTable.RefreshData();
            if (refreshState == PivotRefreshState.Success)
            {
                Console.WriteLine("Pivot table refreshed successfully");
            }
            else if (refreshState == PivotRefreshState.UnsupportedExternalDataSource)
            {
                Console.WriteLine("External data source not supported - calculating data instead");
                pivotTable.CalculateData();
            }

            // Enregistrez le classeur
            workbook.Save("PivotRefreshStateDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


