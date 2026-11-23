---
title: "SqlScriptSaveOptions.CheckIfTableExists"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SqlScriptSaveOptions. Vérifie si le nom de la table existe avant la création"
type: docs
url: /fr/net/aspose.cells.saving/sqlscriptsaveoptions/checkiftableexists/
---
## SqlScriptSaveOptions.CheckIfTableExists property

Vérifier si le nom de la table existe avant de créer

```csharp
public bool CheckIfTableExists { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCheckIfTableExistsDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec des données de test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Configurer les options d'enregistrement SQL
            SqlScriptSaveOptions sqlOptions = new SqlScriptSaveOptions();
            sqlOptions.CreateTable = true;
            sqlOptions.CheckIfTableExists = true;
            sqlOptions.OperatorType = SqlScriptOperatorType.Insert;

            // Enregistrer dans un fichier de script SQL
            workbook.Save("output.sql", sqlOptions);

            // Lire et afficher le SQL généré
            string sqlScript = System.IO.File.ReadAllText("output.sql");
            Console.WriteLine("Generated SQL Script:");
            Console.WriteLine(sqlScript);
        }
    }
}
```

### Voir aussi

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


