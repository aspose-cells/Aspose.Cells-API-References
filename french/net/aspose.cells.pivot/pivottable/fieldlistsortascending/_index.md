---
title: "PivotTable.FieldListSortAscending"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotTable. Indique si les champs du PivotTable sont triés dans un ordre non par défaut dans la liste de champs"
type: docs
url: /fr/net/aspose.cells.pivot/pivottable/fieldlistsortascending/
---
## PivotTable.FieldListSortAscending property

Indique si les champs du tableau croisé dynamique sont triés dans un ordre non par défaut dans la liste des champs.

```csharp
public bool FieldListSortAscending { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyFieldListSortAscendingDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le tableau croisé dynamique
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Product";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["B2"].Value = "Laptop";
            worksheet.Cells["C2"].Value = 1200;
            
            worksheet.Cells["A3"].Value = "Electronics";
            worksheet.Cells["B3"].Value = "Phone";
            worksheet.Cells["C3"].Value = 800;
            
            worksheet.Cells["A4"].Value = "Furniture";
            worksheet.Cells["B4"].Value = "Chair";
            worksheet.Cells["C4"].Value = 150;
            
            worksheet.Cells["A5"].Value = "Furniture";
            worksheet.Cells["B5"].Value = "Table";
            worksheet.Cells["C5"].Value = 250;

            // Créer un tableau croisé dynamique
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Ajouter des champs au tableau croisé dynamique
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Afficher la valeur actuelle de FieldListSortAscending
            Console.WriteLine("Initial FieldListSortAscending: " + pivotTable.FieldListSortAscending);

            // Afficher la liste de champs par ordre croissant
            pivotTable.FieldListSortAscending = true;
            Console.WriteLine("FieldListSortAscending set to: " + pivotTable.FieldListSortAscending);

            // Actualisez et calculez le tableau croisé dynamique
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Enregistrez le classeur
            workbook.Save("PivotTableFieldListSortAscendingDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


