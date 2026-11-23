---
title: "JsonSaveOptions.SkipEmptyRows"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonSaveOptions. Indique s'il faut sauter les lignes vides"
type: docs
url: /fr/net/aspose.cells/jsonsaveoptions/skipemptyrows/
---
## JsonSaveOptions.SkipEmptyRows property

Indique s’il faut sauter les lignes vides.

```csharp
public bool SkipEmptyRows { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class JsonSaveOptionsPropertySkipEmptyRowsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Données d'exemple - ajoutez quelques cellules avec des valeurs et laissez certaines lignes vides
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            // Laisser la ligne 3 vide
            worksheet.Cells["A4"].PutValue("Data3");
            worksheet.Cells["B4"].PutValue("Data4");

            // Configurer les options d'enregistrement JSON avec SkipEmptyRows
            JsonSaveOptions saveOptions = new JsonSaveOptions();
            saveOptions.SkipEmptyRows = true; // This will skip the empty row 3
            
            // Enregistrer en JSON
            string outputPath = "output.json";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("JSON saved with SkipEmptyRows=true. Empty rows were skipped.");
        }
    }
}
```

### Voir aussi

* class [JsonSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


