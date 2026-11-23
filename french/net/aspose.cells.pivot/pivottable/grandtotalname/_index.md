---
title: "PivotTable.GrandTotalName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Retourne le libellé affiché dans l'en-tête de la colonne ou de la ligne du total général. La valeur par défaut est la chaîne Grand Total"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/grandtotalname/
---
## PivotTable.GrandTotalName property

Renvoie l'étiquette affichée dans l'en-tête de colonne ou de ligne du total général. La valeur par défaut est la chaîne "Grand Total".

```csharp
public string GrandTotalName { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyGrandTotalNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Laptop";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Laptop";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 1500;
            
            worksheet.Cells["A4"].Value = "Phone";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["C4"].Value = 800;
            
            worksheet.Cells["A5"].Value = "Phone";
            worksheet.Cells["B5"].Value = "South";
            worksheet.Cells["C5"].Value = 1200;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Ajouter des champs de ligne et de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Afficher la valeur actuelle de GrandTotalName
            Console.WriteLine("Current GrandTotalName: " + pivotTable.GrandTotalName);

            // Modifier le GrandTotalName
            pivotTable.GrandTotalName = "Total Summary";

            // Calculer les données et actualiser le tableau croisé dynamique
            pivotTable.CalculateData();
            pivotTable.RefreshData();

            // Enregistrez le classeur
            workbook.Save("PivotTableGrandTotalNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


