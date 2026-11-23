---
title: "PivotTable.ShowDetail"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTable. Afficher le détail d'un élément dans la région de données vers une nouvelle Table"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/showdetail/
---
## PivotTable.ShowDetail method

Affiche le détail d'un élément dans la région de données dans un nouveau tableau.

```csharp
public void ShowDetail(int rowOffset, int columnOffset, bool newSheet, int destRow, int destColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | Décalage jusqu'à la première ligne de données dans la région de données. |
| columnOffset | Int32 | Décalage jusqu'à la première colonne de données dans la région de données. |
| newSheet | Boolean | Afficher le détail dans une nouvelle feuille de calcul. |
| destRow | Int32 | La ligne cible. |
| destColumn | Int32 | La colonne cible. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowDetailWithInt32Int32BooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Sport");
            worksheet.Cells["A2"].PutValue("Tennis");
            worksheet.Cells["A3"].PutValue("Basketball");
            worksheet.Cells["A4"].PutValue("Tennis");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(80);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(85);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Sport");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Score");

            // Afficher le détail pour une cellule spécifique
            pivotTable.ShowDetail(1, 0, true, 0, 0);

            // Enregistrez le classeur
            workbook.Save("PivotTableShowDetailExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


