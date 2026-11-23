---
title: "JsonLoadOptions.JsonLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur de JsonLoadOptions. Crée des options de chargement du fichier"
type: docs
url: /fr/net/aspose.cells/jsonloadoptions/jsonloadoptions/
---
## JsonLoadOptions constructor

Crée une option de chargement du fichier.

```csharp
public JsonLoadOptions()
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Répertoires source et de sortie
            string sourceDir = "SourceDir/";
            string outputDir = "OutputDir/";
            
            // Créer JsonLoadOptions en utilisant le constructeur
            JsonLoadOptions loadOptions = new JsonLoadOptions();
            loadOptions.KeptSchema = true;

            // Charger le fichier JSON avec les options
            Workbook workbook = new Workbook(sourceDir + "example.json", loadOptions);
            
            // Enregistrer en tant que fichier Excel
            workbook.Save(outputDir + "example.xlsx");

            // Enregistrer à nouveau en JSON avec JsonSaveOptions
            workbook.Save(outputDir + "example_output.json", new JsonSaveOptions()
            {
                ExportNestedStructure = true,
                SkipEmptyRows = true
            });

            Console.WriteLine("JSON to Excel conversion completed successfully.");
        }
    }
}
```

### Voir aussi

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


