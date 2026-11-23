---
title: "PivotPageFields.PageFieldCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PivotPageFields. Obtient le nombre de champs de page"
type: docs
url: /fr/net/aspose.cells.pivot/pivotpagefields/pagefieldcount/
---
## PivotPageFields.PageFieldCount property

Obtient le nombre de champs de page.

```csharp
public int PageFieldCount { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsPropertyPageFieldCountDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer des feuilles de calcul d'exemple avec des données
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "Data1";
            FillSampleData(sheet1);

            Worksheet sheet2 = workbook.Worksheets.Add("Data2");
            FillSampleData(sheet2);

            // Créer une feuille pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");

            // Créer une instance de PivotPageFields
            PivotPageFields pageFields = new PivotPageFields();

            // Ajouter des champs de page pour démontrer la propriété PageFieldCount
            pageFields.AddPageField(new string[] { "Category1", "Category2" });
            pageFields.AddPageField(new string[] { "Region1", "Region2" });

            try
            {
                // Afficher la valeur de la propriété PageFieldCount
                Console.WriteLine("Number of page fields: " + pageFields.PageFieldCount);

                // Ajouter une identification pour les champs de page
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                pageFields.AddIdentify(1, new int[] { 1, 0 });

                // Vérifier que le nombre reste le même après l'ajout des identifications
                Console.WriteLine("PageFieldCount after adding identifications: " + pageFields.PageFieldCount);

                // Créer un tableau croisé dynamique en utilisant les champs de page
                string[] sources = { "=Data1!A1:C4", "=Data2!A1:C4" };
                pivotSheet.PivotTables.Add(sources, false, pageFields, "E3", "DemoPivot");

                // Enregistrez le classeur
                workbook.Save("PageFieldCountDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private static void FillSampleData(Worksheet sheet)
        {
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Region");
            cells["C1"].PutValue("Value");

            cells["A2"].PutValue("Category1");
            cells["B2"].PutValue("Region1");
            cells["C2"].PutValue(100);

            cells["A3"].PutValue("Category2");
            cells["B3"].PutValue("Region2");
            cells["C3"].PutValue(200);
        }
    }
}
```

### Voir aussi

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


