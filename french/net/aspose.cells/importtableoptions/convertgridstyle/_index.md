---
title: "ImportTableOptions.ConvertGridStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImportTableOptions. Indique si le style de la vue grille doit être appliqué aux cellules"
type: docs
url: /fr/net/aspose.cells/importtableoptions/convertgridstyle/
---
## ImportTableOptions.ConvertGridStyle property

Indique si le style de la vue grille doit être appliqué aux cellules.

```csharp
public bool ConvertGridStyle { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyConvertGridStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer des données d'exemple
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            dataTable.Rows.Add(101, "Laptop", 999.99m);
            dataTable.Rows.Add(102, "Monitor", 249.50m);

            // Définir les options d'importation avec ConvertGridStyle activé
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertGridStyle = true; // This will apply grid styling to the imported data
            options.IsFieldNameShown = true;

            // Importer des données avec mise en forme
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // Enregistrer le résultat
            workbook.Save("ImportWithGridStyle.xlsx");
        }
    }
}
```

### Voir aussi

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


