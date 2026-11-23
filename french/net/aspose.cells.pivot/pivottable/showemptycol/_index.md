---
title: "PivotTable.ShowEmptyCol"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique s'il faut inclure des colonnes vides dans le tableau"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/showemptycol/
---
## PivotTable.ShowEmptyCol property

Indique s'il faut inclure des colonnes vides dans le tableau

```csharp
public bool ShowEmptyCol { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyShowEmptyColDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Afficher la valeur actuelle de ShowEmptyCol
            Console.WriteLine("Current ShowEmptyCol value: " + pivotTable.ShowEmptyCol);

            // Définir ShowEmptyCol sur false (masquer les colonnes vides)
            pivotTable.ShowEmptyCol = false;
            Console.WriteLine("ShowEmptyCol set to false - empty columns will be hidden");

            // Calculer les données du tableau croisé dynamique
            pivotTable.CalculateData();

            // Enregistrer le classeur avec des colonnes vides masquées
            workbook.Save("PivotTableHideEmptyCols.xlsx");

            // Redéfinir ShowEmptyCol sur true (afficher les colonnes vides)
            pivotTable.ShowEmptyCol = true;
            Console.WriteLine("ShowEmptyCol set to true - empty columns will be shown");

            // Recalculer les données du tableau croisé dynamique
            pivotTable.CalculateData();

            // Enregistrer le classeur avec des colonnes vides visibles
            workbook.Save("PivotTableShowEmptyCols.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


