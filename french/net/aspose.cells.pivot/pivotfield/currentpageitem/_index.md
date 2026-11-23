---
title: "PivotField.CurrentPageItem"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotField. Obtient ou définit l'élément de page actuellement affiché pour ce champ de tableau croisé dynamique, uniquement le champ de page."
type: docs
url: /fr/net/aspose.cells.pivot/pivotfield/currentpageitem/
---
## PivotField.CurrentPageItem property

Obtient ou définit l'élément de page actuellement affiché pour ce champ pivot (champ de page uniquement).

```csharp
public short CurrentPageItem { get; set; }
```

### Remarques

Utilisez [`AllPageItemsIndex`](../../pivotitem/allpageitemsindex/) (0x7FFD) comme valeur sentinelle pour indiquer « Select All ». Il s'agit d'un marqueur prédéfini et ce n'est pas un indice d'élément valide.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyCurrentPageItemDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Apple";
            worksheet.Cells["A5"].Value = "Orange";
            
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["B4"].Value = "North";
            worksheet.Cells["B5"].Value = "East";
            
            worksheet.Cells["C1"].Value = "Sales";
            worksheet.Cells["C2"].Value = 1000;
            worksheet.Cells["C3"].Value = 2000;
            worksheet.Cells["C4"].Value = 1500;
            worksheet.Cells["C5"].Value = 3000;

            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Ajouter des champs
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Product");
            
            // Rafraîchir les données
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Obtenir les champs de page
            PivotFieldCollection pageFields = pivotTable.PageFields;
            
            // Afficher les éléments de page actuels
            Console.WriteLine("Initial CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // Modifier l'élément de page actuel
            pageFields[0].CurrentPageItem = 1; // Change to Banana
            Console.WriteLine("After Change CurrentPageItem: " + pageFields[0].CurrentPageItem);
            
            // Enregistrez le classeur
            workbook.Save("PivotFieldCurrentPageItemDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


