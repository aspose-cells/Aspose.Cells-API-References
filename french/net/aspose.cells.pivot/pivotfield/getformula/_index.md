---
title: "PivotField.GetFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotField. Obtient la formule du champ calculé. Fonctionne uniquement pour le champ calculé"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/getformula/
---
## PivotField.GetFormula method

Obtient la formule du champ calculé. Fonctionne uniquement pour le champ calculé.

```csharp
public string GetFormula()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodGetFormulaDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Bike";
            worksheet.Cells["B4"].Value = 1500;
            
            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter un champ calculé avec une formule
            pivotTable.AddCalculatedField("=ABS('Sales')", "Absolute Sales");
            
            // Obtenir la formule du champ calculé
            PivotFieldCollection fields = pivotTable.DataFields;
            string formula = fields[fields.Count - 1].GetFormula();
            
            // Afficher la formule
            Console.WriteLine("Calculated field formula: " + formula);
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


