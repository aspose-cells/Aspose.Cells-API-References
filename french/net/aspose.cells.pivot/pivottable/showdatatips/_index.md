---
title: "PivotTable.ShowDataTips"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si les infobulles doivent être affichées pour les cellules de données du tableau croisé dynamique"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/showdatatips/
---
## PivotTable.ShowDataTips property

Indique si les infobulles doivent être affichées pour les cellules de données du PivotTable.

```csharp
public bool ShowDataTips { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowDataTipsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul et des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 20;

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Configurer le tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Activer les infobulles
            pivotTable.ShowDataTips = true;
            
            // Enregistrez le classeur
            workbook.Save("PivotTableWithDataTips.xlsx");
            
            Console.WriteLine("Pivot table with ShowDataTips enabled created successfully.");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


