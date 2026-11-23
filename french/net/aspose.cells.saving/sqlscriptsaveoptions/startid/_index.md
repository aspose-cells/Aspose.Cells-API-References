---
title: "SqlScriptSaveOptions.StartId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SqlScriptSaveOptions. Obtient et définit l'ID de départ"
type: docs
url: /fr/net/aspose.cells.saving/sqlscriptsaveoptions/startid/
---
## SqlScriptSaveOptions.StartId property

Obtient et définit l'identifiant de départ.

```csharp
public int StartId { get; set; }
```

### Remarques

Ne fonctionne que lorsque [`IdName`](../idname/) est défini.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyStartIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // Configurer les options d'exportation SQL avec StartId défini à 100
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                IdName = "ID",
                StartId = 100, // Demonstrating StartId property
                HasHeaderRow = true,
                OperatorType = SqlScriptOperatorType.Insert
            };

            // Enregistrer en tant que script SQL
            workbook.Save("Employees_WithStartId.sql", saveOptions);
        }
    }
}
```

### Voir aussi

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


