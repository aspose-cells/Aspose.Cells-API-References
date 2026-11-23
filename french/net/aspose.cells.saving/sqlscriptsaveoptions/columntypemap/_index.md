---
title: "SqlScriptSaveOptions.ColumnTypeMap"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SqlScriptSaveOptions. Obtient et définit la correspondance des types de colonnes pour différentes bases de données"
type: docs
url: /fr/net/aspose.cells.saving/sqlscriptsaveoptions/columntypemap/
---
## SqlScriptSaveOptions.ColumnTypeMap property

Obtient et définit la correspondance du type de colonne pour différentes bases de données.

```csharp
public SqlScriptColumnTypeMap ColumnTypeMap { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyColumnTypeMapDemo
    {
        public static void Run()
        {
            // Créer une correspondance de type de colonne personnalisée
            SqlScriptColumnTypeMap customTypeMap = new SqlScriptColumnTypeMap();
            
            // Créer des options d’enregistrement SQL
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                CreateTable = true,
                ColumnTypeMap = customTypeMap,
                CheckIfTableExists = true,
                ExportAsString = false
            };

            // Créer un classeur d’exemple avec des données
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des en-têtes
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Salary");
            
            // Ajouter des lignes de données
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Smith");
            worksheet.Cells["C2"].PutValue(5000.50);
            
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane Doe");
            worksheet.Cells["C3"].PutValue(6500.75);

            // Enregistrer en tant que script SQL
            workbook.Save("EmployeeData.sql", saveOptions);
            
            Console.WriteLine("SQL script generated successfully with custom column type mapping.");
        }
    }
}
```

### Voir aussi

* class [SqlScriptColumnTypeMap](../../sqlscriptcolumntypemap/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


