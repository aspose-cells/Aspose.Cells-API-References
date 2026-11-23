---
title: "JsonSaveOptions.AlwaysExportAsJsonObject"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonSaveOptions. Indique s’il faut toujours exporter Excel en JSON sous forme d’objet même s’il n’y a qu’une seule feuille de calcul dans le fichier"
type: docs
url: /fr/net/aspose.cells/jsonsaveoptions/alwaysexportasjsonobject/
---
## JsonSaveOptions.AlwaysExportAsJsonObject property

Indique s’il faut toujours exporter Excel en JSON sous forme d’objet, même s’il n’y a qu’une seule feuille de calcul dans le fichier.

```csharp
public bool AlwaysExportAsJsonObject { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertyAlwaysExportAsJsonObjectDemo
    {
        public static void Run()
        {
            // Créer un classeur d’exemple avec deux feuilles de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Définir des données d’exemple dans la première feuille de calcul
            Cells cells = workbook.Worksheets[0].Cells;
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Value");
            cells["A2"].PutValue("Item1");
            cells["B2"].PutValue(100);

            // Configurer les options d’enregistrement JSON
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.AlwaysExportAsJsonObject = true;
            saveOptions.ExportNestedStructure = true;
            saveOptions.SkipEmptyRows = true;

            // Enregistrer dans un fichier JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);

            // Afficher le contenu JSON enregistré
            string jsonContent = File.ReadAllText(outputPath);
            Console.WriteLine(jsonContent);
        }
    }
}
```

### Voir aussi

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


