---
title: "PivotField.AutoSortField"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Représente l'index du champ qui est trié automatiquement. 1 signifie le PivotField lui‑même, d'autres valeurs indiquent la position des champs de données."
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/autosortfield/
---
## PivotField.AutoSortField property

Représente l'index du champ qui est trié automatiquement. -1 signifie le PivotField lui‑même, d'autres valeurs indiquent la position des champs de données.

```csharp
[Obsolete("Use PivotField.SortSetting.SortBy property or PivotField.SortBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoSortField { get; set; }
```

### Remarques

NOTE : Cette propriété est maintenant obsolète. Veuillez plutôt utiliser la propriété PivotField.SortSetting.SortBy ou la méthode PivotField.SortBy(). Cette méthode sera supprimée 12 mois plus tard, à compter de septembre 2026. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoSortFieldDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Branch";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "North";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "South";
            cells["B3"].Value = 1500;
            cells["A4"].Value = "East";
            cells["B4"].Value = 800;
            cells["A5"].Value = "West";
            cells["B5"].Value = 1200;

            // Ajouter un tableau croisé dynamique
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Branch");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Obtenez le champ du tableau croisé
            PivotField pivotField = pivotTable.RowFields["Branch"];

            // Configurer le tri automatique
            pivotField.IsAutoSort = true;
            pivotField.IsAscendSort = true;
            pivotField.AutoSortField = 0; // Sort by first data field (Sales)

            // Calculer les données et actualiser
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotFieldAutoSortDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


