---
title: "Enum SqlScriptOperatorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Saving.SqlScriptOperatorType. Représente le type de données opérationnelles"
type: docs
url: /fr/net/aspose.cells.saving/sqlscriptoperatortype/
---
## SqlScriptOperatorType enumeration

Représente le type de données opérationnelles.

```csharp
public enum SqlScriptOperatorType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Insert | `0` | Insérer des données. |
| Update | `1` | Mettre à jour les données. |
| Delete | `2` | Supprimer les données. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptOperatorTypeDemo
    {
        public static void SqlScriptOperatorTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // Créer SqlScriptSaveOptions et définir les propriétés
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                CheckIfTableExists = true,
                AddBlankLineBetweenRows = true,
                Separator = ';',
                OperatorType = SqlScriptOperatorType.Insert,
                PrimaryKey = 0,
                CreateTable = true,
                IdName = "ID",
                StartId = 1,
                TableName = "SampleTable",
                ExportAsString = false,
                ExportArea = new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 1 },
                HasHeaderRow = true
            };

            // Enregistrer le classeur en tant que script SQL
            workbook.Save("SqlScriptOperatorTypeExample.sql", saveOptions);

            // Afficher les résultats
            Console.WriteLine("SQL script has been saved successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


