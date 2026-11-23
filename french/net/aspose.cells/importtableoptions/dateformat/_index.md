---
title: "ImportTableOptions.DateFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ImportTableOptions. Obtient ou définit la chaîne de format de date pour les cellules contenant des valeurs datetime importées"
type: docs
url: /fr/net/aspose.cells/importtableoptions/dateformat/
---
## ImportTableOptions.DateFormat property

Obtient ou définit la chaîne de format de date pour les cellules contenant des valeurs datetime importées.

```csharp
public string DateFormat { get; set; }
```

### Exemples

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un DataTable d'exemple avec des valeurs de date
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("DateColumn", typeof(DateTime));
            dataTable.Rows.Add(new DateTime(2023, 1, 15));
            dataTable.Rows.Add(new DateTime(2023, 2, 20));
            dataTable.Rows.Add(new DateTime(2023, 3, 25));

            // Définir la plage d'importation
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 10, 1);

            // Importer des données avec un format de date personnalisé
            worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions()
            {
                IsFieldNameShown = true,
                DateFormat = "YYYY-MM-DD"
            });

            // Enregistrer le classeur pour démontrer le résultat
            workbook.Save("DateFormatDemoOutput.xlsx");
        }
    }
}
```

### Voir aussi

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


