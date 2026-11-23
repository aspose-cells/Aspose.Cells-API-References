---
title: "PivotItem.GetFormula"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotItem. Obtient la formule de cet élément calculé. Fonctionne uniquement lorsque cet élément est un élément calculé"
type: docs
url: /fr/net/aspose.cells.pivot/pivotitem/getformula/
---
## PivotItem.GetFormula method

Obtient la formule de cet élément calculé. Fonctionne uniquement lorsque cet élément est un élément calculé.

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
    public class PivotItemMethodGetFormulaDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Ajouter un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter le champ de ligne et le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Calculer les données
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Obtenez la formule des éléments pivot
            string rowItemFormula = pivotTable.RowFields[0].PivotItems[0].GetFormula();
            string dataFieldFormula = pivotTable.DataFields[0].GetFormula();

            Console.WriteLine("Row Item Formula: " + rowItemFormula);
            Console.WriteLine("Data Field Formula: " + dataFieldFormula);
        }
    }
}
```

### Voir aussi

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


