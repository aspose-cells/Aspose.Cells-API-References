---
title: "SqlScriptSaveOptions.IdName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SqlScriptSaveOptions. Obtient et définit le nom de la colonne d’identifiant"
type: docs
url: /fr/net/aspose.cells.saving/sqlscriptsaveoptions/idname/
---
## SqlScriptSaveOptions.IdName property

Obtient et définit le nom de la colonne d'identifiant.

```csharp
public string IdName { get; set; }
```

### Remarques

Si cette propriété est définie, une colonne sera insérée avec une valeur entière incrémentée automatiquement.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyIdNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");

            // Configurer les options d’exportation SQL avec IdName
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                IdName = "ID",
                CreateTable = true,
                HasHeaderRow = true
            };

            // Enregistrer en tant que script SQL
            workbook.Save("Employees.sql", saveOptions);

            Console.WriteLine("SQL script exported with IdName property");
        }
    }
}
```

### Voir aussi

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


