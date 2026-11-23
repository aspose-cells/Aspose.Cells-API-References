---
title: "Enum RenameStrategy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.RenameStrategy enum. Option de stratégie pour les noms en double des colonnes"
type: docs
url: /fr/net/aspose.cells/renamestrategy/
---
## RenameStrategy enumeration

Option de stratégie pour les noms de colonnes en double.

```csharp
public enum RenameStrategy
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Exception | `0` | Lance une exception. |
| Digit | `1` | Nommé avec un chiffre. Les noms dupliqués deviendront ...1, ...2, etc. |
| Letter | `2` | Nommé avec une lettre.. Les noms dupliqués deviendront ...A, ...B, etc. |

### Remarques

Lors du traitement des données avec des en-têtes, certains scénarios exigent que les en-têtes ne soient pas dupliqués pour toutes les colonnes. Par exemple, lors de l'exportation de données vers un DataTable et que l'en-tête doit être utilisé comme nom de colonne du DataTable, les valeurs d'en-tête dupliquées sont invalides. Dans ce type de situation, l'utilisateur peut déterminer comment les gérer en spécifiant cette stratégie.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RenameStrategyDemo
    {
        public static void RenameStrategyExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("John");

            // Créez ExportTableOptions et définissez le RenameStrategy
            ExportTableOptions options = new ExportTableOptions
            {
                RenameStrategy = RenameStrategy.Digit // Use the Digit strategy for duplicate names
            };

            // Exportez les données de la feuille de calcul vers un DataTable
            System.Data.DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 1, options);

            // Affichez le contenu du DataTable
            foreach (System.Data.DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Enregistrez le classeur
            workbook.Save("RenameStrategyExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


