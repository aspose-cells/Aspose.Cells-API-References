---
title: "Enum PivotAreaType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Pivot.PivotAreaType. Indique le type de règle utilisé pour décrire une zone ou un aspect du tableau croisé dynamique."
type: docs
url: /fr/net/aspose.cells.pivot/pivotareatype/
---
## PivotAreaType enumeration

Indique le type de règle utilisé pour décrire une zone ou un aspect du **PivotTable**.

```csharp
public enum PivotAreaType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| None | `0` | Aucune zone de Pivot. |
| Normal | `1` | Représente un en‑tête ou un élément. |
| Data | `2` | Représente quelque chose dans la zone de données. |
| All | `3` | Représente l'ensemble du tableau croisé dynamique. |
| Origin | `4` | Représente les cellules vides en haut à gauche du tableau croisé dynamique (en haut à droite pour les feuilles RTL). |
| Button | `5` | Représente un bouton de champ. |
| TopRight | `6` | Représente les cellules vides en haut à droite du tableau croisé dynamique (en haut à gauche pour les feuilles RTL). |

### Exemples

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotAreaTypeDemo
    {
        public static void PivotAreaTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["A4"].PutValue("Bananas");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);

            // Créer un tableau croisé dynamique
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Ajoutez des champs au PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Créer une PivotArea pour le tableau croisé dynamique
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true;
            pivotArea.IsRowGrandIncluded = true;

            // Afficher les propriétés de la PivotArea
            Console.WriteLine("Pivot Area Type: " + pivotArea.RuleType);
            Console.WriteLine("Only Data: " + pivotArea.OnlyData);
            Console.WriteLine("Is Row Grand Included: " + pivotArea.IsRowGrandIncluded);

            // Enregistrez le classeur
            workbook.Save("PivotAreaTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


