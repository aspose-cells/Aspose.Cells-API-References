---
title: "SqlScriptSaveOptions.SqlScriptSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur SqlScriptSaveOptions. Crée des options pour enregistrer un fichier sql"
type: docs
url: /fr/net/aspose.cells.saving/sqlscriptsaveoptions/sqlscriptsaveoptions/
---
## SqlScriptSaveOptions constructor

Crée des options pour l'enregistrement du fichier SQL.

```csharp
public SqlScriptSaveOptions()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Créer SqlScriptSaveOptions à l'aide du constructeur
            SqlScriptSaveOptions options = new SqlScriptSaveOptions();
            options.OperatorType = SqlScriptOperatorType.Insert;
            options.AddBlankLineBetweenRows = true;

            // Enregistrer en tant que script SQL
            workbook.Save("output.sql", options);
            
            // Afficher le SQL généré
            Console.WriteLine("Generated SQL Script:");
            Console.WriteLine(System.IO.File.ReadAllText("output.sql"));
        }
    }
}
```

### Voir aussi

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


