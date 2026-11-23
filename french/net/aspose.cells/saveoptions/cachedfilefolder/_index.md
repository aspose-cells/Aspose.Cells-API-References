---
title: "SaveOptions.CachedFileFolder"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SaveOptions. Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données"
type: docs
url: /fr/net/aspose.cells/saveoptions/cachedfilefolder/
---
## SaveOptions.CachedFileFolder property

Le dossier pour les fichiers temporaires pouvant être utilisés comme cache de données.

```csharp
public string CachedFileFolder { get; set; }
```

### Remarques

Si le dossier n’a pas été spécifié, la valeur par défaut est [`GetCacheFolder`](../../cellshelper/getcachefolder/). Si sa valeur par défaut est null ou vide, ou a été spécifiée comme null ou vide, alors aucun fichier de cache ne sera utilisé lors de l’enregistrement du classeur.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCachedFileFolderDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test cached file folder");

            // Définir les options d’enregistrement avec le dossier de fichiers en cache
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.CachedFileFolder = "TempCache"; // Specify cache folder

            // Enregistrez le classeur
            workbook.Save("output.xml", saveOptions);
            
            Console.WriteLine("File saved with cached file folder option.");
        }
    }
}
```

### Voir aussi

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


