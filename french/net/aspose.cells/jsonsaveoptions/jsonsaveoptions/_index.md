---
title: "JsonSaveOptions.JsonSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur JsonSaveOptions. Crée des options pour enregistrer un fichier json"
type: docs
url: /fr/net/aspose.cells/jsonsaveoptions/jsonsaveoptions/
---
## JsonSaveOptions constructor

Crée des options pour l’enregistrement du fichier JSON.

```csharp
public JsonSaveOptions()
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Données d'exemple à exporter en JSON
            workbook.Worksheets[0].Cells["A1"].PutValue("Name");
            workbook.Worksheets[0].Cells["B1"].PutValue("Age");
            workbook.Worksheets[0].Cells["A2"].PutValue("John");
            workbook.Worksheets[0].Cells["B2"].PutValue(30);
            
            // Initialiser JsonSaveOptions en utilisant le constructeur
            JsonSaveOptions options = new JsonSaveOptions();
            
            // Définir les options d'exportation JSON
            options.ExportNestedStructure = true;
            options.SkipEmptyRows = true;
            options.ValidateMergedAreas = true;
            
            // Enregistrer le classeur avec les options JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, options);
            
            Console.WriteLine("JSON file saved successfully with options.");
        }
    }
}
```

### Voir aussi

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


