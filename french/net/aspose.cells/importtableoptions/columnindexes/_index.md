---
title: "ImportTableOptions.ColumnIndexes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImportTableOptions. Obtient ou définit les colonnes indexées à partir de 0 à importer depuis la source de données. null signifie que toutes les colonnes doivent être importées"
type: docs
url: /fr/net/aspose.cells/importtableoptions/columnindexes/
---
## ImportTableOptions.ColumnIndexes property

Obtient ou définit les colonnes (indexées à partir de 0) à importer depuis la source de données. null signifie que toutes les colonnes doivent être importées.

```csharp
public int[] ColumnIndexes { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyColumnIndexesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer un DataTable d’exemple
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // Ajoutez des données d'exemple
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);
            dataTable.Rows.Add(3, "Product C", 39.99m);

            // Définissez les options d'importation pour n'importer que les colonnes aux index 0 et 2 (ID et Prix)
            ImportTableOptions options = new ImportTableOptions();
            options.ColumnIndexes = new int[] { 0, 2 };
            options.IsFieldNameShown = true;

            // Importer des données avec les index de colonnes spécifiés
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // Enregistrez le classeur
            workbook.Save("ColumnIndexesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


