---
title: "ImportTableOptions.DefaultValues"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImportTableOptions. La valeur par défaut pour la valeur dans le tableau est null"
type: docs
url: /fr/net/aspose.cells/importtableoptions/defaultvalues/
---
## ImportTableOptions.DefaultValues property

La valeur par défaut pour la valeur dans le tableau est null.

```csharp
public object[] DefaultValues { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsPropertyDefaultValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple avec des valeurs nulles
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Quantity", typeof(int));
            dataTable.Columns.Add("ExpiryDate", typeof(DateTime));
            
            dataTable.Rows.Add("Bread", 10, DateTime.Now.AddDays(7));
            dataTable.Rows.Add(null, null, null); // Will use default values
            dataTable.Rows.Add("Milk", null, DateTime.Now.AddDays(3));

            ImportTableOptions importOptions = new ImportTableOptions();
            
            // Afficher l'état initial
            Console.WriteLine("Current DefaultValues: " + (importOptions.DefaultValues == null ? "Not set" : "Set"));

            // Configurer les valeurs par défaut pour chaque colonne
            importOptions.DefaultValues = new object[] { "[Unspecified]", 1, DateTime.Today };

            // Importer des données avec gestion des valeurs nulles
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Ajuster automatiquement les colonnes pour une meilleure visibilité
            worksheet.AutoFitColumns();

            workbook.Save("DefaultValuesDemo.xlsx");
            Console.WriteLine("Spreadsheet saved with default values applied to null entries.");
        }
    }
}
```

### Voir aussi

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


