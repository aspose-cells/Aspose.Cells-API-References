---
title: "SaveOptions.CreateDirectory"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SaveOptions. Si true et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant d'enregistrer le fichier"
type: docs
url: /fr/net/aspose.cells/saveoptions/createdirectory/
---
## SaveOptions.CreateDirectory property

Si vrai et que le répertoire n'existe pas, le répertoire sera créé automatiquement avant l'enregistrement du fichier.

```csharp
public bool CreateDirectory { get; set; }
```

### Remarques

La valeur par défaut est false.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCreateDirectoryDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Définir les options d'enregistrement avec CreateDirectory activé
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.CreateDirectory = true;

            // Enregistrer le classeur dans un nouveau répertoire (qui sera créé automatiquement)
            string outputPath = "OutputDirectory/example.xls";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved successfully with directory creation.");
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


