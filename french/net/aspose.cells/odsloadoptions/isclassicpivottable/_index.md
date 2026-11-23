---
title: "OdsLoadOptions.IsClassicPivotTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OdsLoadOptions. Indique si le tableau croisé dynamique est classique"
type: docs
url: /fr/net/aspose.cells/odsloadoptions/isclassicpivottable/
---
## OdsLoadOptions.IsClassicPivotTable property

Indique si le tableau croisé dynamique est classique.

```csharp
public bool IsClassicPivotTable { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class OdsLoadOptionsPropertyIsClassicPivotTableDemo
    {
        public static void Run()
        {
            // Créer un fichier ODS d'exemple avec un tableau croisé dynamique
            CreateSampleOdsWithPivotTable();

            // Charger avec IsClassicPivotTable défini sur true
            OdsLoadOptions loadOptionsTrue = new OdsLoadOptions();
            loadOptionsTrue.IsClassicPivotTable = true;
            
            Workbook workbookTrue = new Workbook("SamplePivot.ods", loadOptionsTrue);
            Console.WriteLine("Loaded with IsClassicPivotTable = true");
            Console.WriteLine("PivotTable fields count: " + workbookTrue.Worksheets[0].PivotTables[0].BaseFields.Count);

            // Charger avec IsClassicPivotTable défini sur false
            OdsLoadOptions loadOptionsFalse = new OdsLoadOptions();
            loadOptionsFalse.IsClassicPivotTable = false;
            
            Workbook workbookFalse = new Workbook("SamplePivot.ods", loadOptionsFalse);
            Console.WriteLine("\nLoaded with IsClassicPivotTable = false");
            Console.WriteLine("PivotTable fields count: " + workbookFalse.Worksheets[0].PivotTables[0].BaseFields.Count);
        }

        private static void CreateSampleOdsWithPivotTable()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Remplissez des données d'exemple
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Electronics";
            cells["A3"].Value = "Clothing";
            cells["A4"].Value = "Books";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1500;
            cells["B3"].Value = 800;
            cells["B4"].Value = 200;

            // Créer un tableau croisé dynamique
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesReport");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Ajouter un champ de ligne (Category)
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            
            // Ajouter un champ de données (Sales) et définir le nom d'affichage
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.DataFields[dataFieldIndex].DisplayName = "Total Sales";

            // Enregistrer sous ODS
            workbook.Save("SamplePivot.ods", SaveFormat.Ods);
        }
    }
}
```

### Voir aussi

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


