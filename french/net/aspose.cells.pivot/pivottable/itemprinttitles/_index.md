---
title: "PivotTable.ItemPrintTitles"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si les noms de PivotItem doivent être répétés en haut de chaque page imprimée"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/itemprinttitles/
---
## PivotTable.ItemPrintTitles property

Indique si les noms de PivotItem doivent être répétés en haut de chaque page imprimée.

```csharp
[Obsolete("Use PivotTable.RepeatItemsOnEachPrintedPage property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ItemPrintTitles { get; set; }
```

### Remarques

NOTE : Cette propriété est désormais obsolète. Veuillez plutôt utiliser la propriété PivotTable.RepeatItemsOnEachPrintedPage. Cette méthode sera supprimée 12 mois après octobre 2024. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyItemPrintTitlesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);
            worksheet.Cells["A5"].PutValue("Product D");
            worksheet.Cells["B5"].PutValue("West");
            worksheet.Cells["C5"].PutValue(4000);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Afficher la valeur actuelle de ItemPrintTitles
            Console.WriteLine("Current ItemPrintTitles value: " + pivotTable.ItemPrintTitles);

            // Définir ItemPrintTitles sur true (cette propriété est obsolète, mais affichée à titre d'exemple)
            pivotTable.ItemPrintTitles = true;

            // Sinon, utilisez la propriété non obsolète
            pivotTable.RepeatItemsOnEachPrintedPage = true;

            // Actualisez et calculez le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotTableItemPrintTitlesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


