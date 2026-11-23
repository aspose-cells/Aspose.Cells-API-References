---
title: "SqlScriptSaveOptions.SheetIndexes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SqlScriptSaveOptions. Représente les index des feuilles exportées"
type: docs
url: /fr/net/aspose.cells.saving/sqlscriptsaveoptions/sheetindexes/
---
## SqlScriptSaveOptions.SheetIndexes property

Représente les index des feuilles exportées.

```csharp
public int[] SheetIndexes { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptSaveOptionsPropertySheetIndexesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec plusieurs feuilles
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Remplir des données dans toutes les feuilles
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet worksheet = workbook.Worksheets[i];
                worksheet.Cells["A1"].PutValue("ID");
                worksheet.Cells["B1"].PutValue("Name");
                worksheet.Cells["A2"].PutValue(1);
                worksheet.Cells["B2"].PutValue("John");
                worksheet.Cells["A3"].PutValue(2);
                worksheet.Cells["B3"].PutValue("Jane");
            }

            // Créer une instance de SqlScriptSaveOptions
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Afficher les SheetIndexes actuels (null signifie toutes les feuilles)
            Console.WriteLine("Initial SheetIndexes: " + 
                (options.SheetIndexes == null ? "All sheets" : string.Join(",", options.SheetIndexes)));

            // Définir SheetIndexes pour n’exporter que les première et troisième feuilles (0 et 2)
            options.SheetIndexes = new int[] { 0, 2 };

            // Enregistrer avec les options
            workbook.Save("SqlScriptExportSelectedSheets.sql", options);

            // Modifier SheetIndexes pour n’exporter que la deuxième feuille
            options.SheetIndexes = new int[] { 1 };
            workbook.Save("SqlScriptExportSecondSheet.sql", options);

            // Définir SheetIndexes à null pour exporter toutes les feuilles
            options.SheetIndexes = null;
            workbook.Save("SqlScriptExportAllSheets.sql", options);
        }
    }
}
```

### Voir aussi

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


