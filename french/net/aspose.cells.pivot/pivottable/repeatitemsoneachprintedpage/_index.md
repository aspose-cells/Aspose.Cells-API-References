---
title: "PivotTable.RepeatItemsOnEachPrintedPage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si les légendes des éléments de tableau croisé dynamique dans la zone de lignes sont répétées sur chaque page imprimée pour les champs de tableau croisé dynamique sous forme tabulaire"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/repeatitemsoneachprintedpage/
---
## PivotTable.RepeatItemsOnEachPrintedPage property

Indique si les légendes des éléments de tableau croisé dynamique dans la zone de lignes sont répétées sur chaque page imprimée pour les champs de tableau croisé dynamique sous forme tabulaire.

```csharp
public bool RepeatItemsOnEachPrintedPage { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyRepeatItemsOnEachPrintedPageDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["A2"].PutValue("North");
            worksheet.Cells["A3"].PutValue("North");
            worksheet.Cells["A4"].PutValue("South");
            worksheet.Cells["A5"].PutValue("South");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["B2"].PutValue("Apples");
            worksheet.Cells["B3"].PutValue("Oranges");
            worksheet.Cells["B4"].PutValue("Apples");
            worksheet.Cells["B5"].PutValue("Oranges");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["C3"].PutValue(1500);
            worksheet.Cells["C4"].PutValue(2000);
            worksheet.Cells["C5"].PutValue(2500);

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Ajouter des champs de ligne et le champ de données
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Définir la configuration de page pour l'impression
            worksheet.PageSetup.PrintTitleRows = "$1:$1";
            worksheet.PageSetup.PrintArea = "A1:G20";
            worksheet.PageSetup.FitToPagesTall = 0;
            worksheet.PageSetup.FitToPagesWide = 1;

            // Afficher la valeur actuelle de RepeatItemsOnEachPrintedPage
            Console.WriteLine("Current RepeatItemsOnEachPrintedPage value: " + pivotTable.RepeatItemsOnEachPrintedPage);

            // Activer la répétition des éléments sur chaque page imprimée
            pivotTable.RepeatItemsOnEachPrintedPage = true;
            Console.WriteLine("RepeatItemsOnEachPrintedPage set to: " + pivotTable.RepeatItemsOnEachPrintedPage);

            // Calculer les données pour remplir le tableau croisé dynamique
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotTableRepeatItemsOnEachPrintedPageDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


