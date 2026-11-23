---
title: "PivotTable.MergeLabels"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Obtient ou définit s’il faut fusionner les étiquettes de champs ligne/colonne qui s’étendent sur plusieurs cellules"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/mergelabels/
---
## PivotTable.MergeLabels property

Obtient ou définit s'il faut fusionner les étiquettes de champs ligne/colonne qui s'étendent sur plusieurs cellules.

```csharp
public bool MergeLabels { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyMergeLabelsDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Apple";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Orange";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 8;
            worksheet.Cells["B5"].Value = 12;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Ajouter le champ de ligne et le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Activer la fusion des étiquettes
            pivotTable.MergeLabels = true;
            
            // Enregistrez le classeur
            workbook.Save("PivotTableMergeLabelsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


