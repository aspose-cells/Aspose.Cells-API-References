---
title: "SqlScriptColumnTypeMap.GetStringType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SqlScriptColumnTypeMap. Obtient le type de chaîne dans la base de données"
type: docs
url: /fr/net/aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/
---
## SqlScriptColumnTypeMap.GetStringType method

Obtient le type chaîne dans la base de données.

```csharp
public virtual string GetStringType()
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptColumnTypeMapMethodGetStringTypeDemo
    {
        public static void Run()
        {
            // Créez une instance de SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Obtenir et afficher le type de chaîne par défaut
            string stringType = columnTypeMap.GetStringType();
            Console.WriteLine("Default String Type: " + stringType);

            // Créer un classeur simple avec des données de chaîne
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John Doe");

            // Enregistrer avec les options de script SQL en utilisant le mappage des types
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };
            
            workbook.Save("SqlScriptOutput.sql", saveOptions);
            Console.WriteLine("SQL script saved with string type: " + stringType);
        }
    }
}
```

### Voir aussi

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


