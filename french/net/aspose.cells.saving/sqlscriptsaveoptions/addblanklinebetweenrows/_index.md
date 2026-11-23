---
title: "SqlScriptSaveOptions.AddBlankLineBetweenRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SqlScriptSaveOptions. Insère une ligne vide entre chaque donnée"
type: docs
url: /fr/net/aspose.cells.saving/sqlscriptsaveoptions/addblanklinebetweenrows/
---
## SqlScriptSaveOptions.AddBlankLineBetweenRows property

Insérer une ligne vide entre chaque donnée.

```csharp
public bool AddBlankLineBetweenRows { get; set; }
```

### Remarques

Si [`Separator`](../separator/) est '\\n', il est préférable de définir cette propriété sur true pour améliorer la lisibilité.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyAddBlankLineBetweenRowsDemo
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
            SqlScriptSaveOptions options = new SqlScriptSaveOptions
            {
                OperatorType = SqlScriptOperatorType.Insert,
                TableName = "Employees",
                IdName = "ID",
                AddBlankLineBetweenRows = true,
                CreateTable = true
            };

            // Enregistrer dans un flux mémoire et obtenir le script SQL sous forme de chaîne
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string sqlScript = reader.ReadToEnd();
                    Console.WriteLine("SQL script generated with blank lines between rows:");
                    Console.WriteLine(sqlScript);
                }
            }
        }
    }
}
```

### Voir aussi

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


