---
title: "ImportTableOptions.InsertRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImportTableOptions. Indique si de nouvelles lignes doivent être ajoutées pour l'importation des enregistrements de données"
type: docs
url: /fr/net/aspose.cells/importtableoptions/insertrows/
---
## ImportTableOptions.InsertRows property

Indique si de nouvelles lignes doivent être ajoutées pour l'importation des enregistrements de données.

```csharp
public bool InsertRows { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyInsertRowsDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Créer une table de données d'exemple
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            dataTable.Rows.Add(1, "Laptop", 999.99);
            dataTable.Rows.Add(2, "Monitor", 249.99);
            dataTable.Rows.Add(3, "Keyboard", 49.99);

            // Ajouter des données existantes à la feuille de calcul (seront décalées vers le bas par l'insertion)
            cells["A1"].PutValue("Existing Data");
            cells["A2"].PutValue(100);

            // Définir les options d'importation avec InsertRows = true
            ImportTableOptions options = new ImportTableOptions();
            options.InsertRows = true; // This will insert new rows instead of overwriting
            options.IsFieldNameShown = true;

            // Importer des données à partir de la ligne 1 (insérera des lignes sous les données existantes)
            cells.ImportData(dataTable, 1, 0, options);

            // Enregistrez le classeur
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


