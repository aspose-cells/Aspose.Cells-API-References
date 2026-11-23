---
title: "PivotField.IsCalculatedField"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Indique si ce champ pivot est un champ calculé"
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/iscalculatedfield/
---
## PivotField.IsCalculatedField property

Indique si ce champ pivot est un champ calculé.

```csharp
public bool IsCalculatedField { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsCalculatedFieldDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // Ajouter un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter un champ calculé
            pivotTable.AddCalculatedField("Profit", "Sales*0.2", true);

            // Vérifiez si le champ est un champ calculé
            PivotField profitField = pivotTable.BaseFields[pivotTable.BaseFields.Count - 1];
            Console.WriteLine("Is Profit field calculated? " + profitField.IsCalculatedField);

            // Enregistrez le classeur
            workbook.Save("PivotField_IsCalculatedField_Example.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


