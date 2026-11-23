---
title: "PivotTable.ShowRowHeaderCaption"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si la légende de l’en-tête de ligne est affichée dans le rapport PivotTable. Indique si les légendes des champs et les listes déroulantes de filtre sont affichées"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/showrowheadercaption/
---
## PivotTable.ShowRowHeaderCaption property

Indique si la légende de l’en-tête de ligne est affichée dans le rapport PivotTable. Indique si les légendes des champs et les listes déroulantes de filtre sont affichées

```csharp
[Obsolete("Use PivotTable.ShowHeaders property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ShowRowHeaderCaption { get; set; }
```

### Remarques

REMARQUE : Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété PivotTable.ShowHeaders. Cette méthode sera supprimée 12 mois plus tard, à compter d’avril 2026. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowRowHeaderCaptionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul et la remplir avec des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Démontrer la propriété ShowRowHeaderCaption
            pivotTable.ShowRowHeaderCaption = true;
            Console.WriteLine("Row Header Caption Visible: " + pivotTable.ShowRowHeaderCaption);
            
            // Enregistrez le classeur
            workbook.Save("PivotTableShowRowHeaderCaptionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


