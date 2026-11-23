---
title: "HtmlSaveOptions.AttachedFilesUrlPrefix"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Spécifiez le préfixe d’URL des fichiers joints tels que les images dans le fichier HTML. uniquement pour l’enregistrement vers un flux HTML"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/attachedfilesurlprefix/
---
## HtmlSaveOptions.AttachedFilesUrlPrefix property

Spécifiez le préfixe d'URL des fichiers joints tels que les images dans le fichier html. Uniquement pour l'enregistrement dans un flux html.

```csharp
public string AttachedFilesUrlPrefix { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAttachedFilesUrlPrefixDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test HTML Export");

            // Définissez les options d’enregistrement HTML avec AttachedFilesUrlPrefix
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.AttachedFilesUrlPrefix = "www.aspose.com";

            // Enregistrer le classeur avec les options HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with AttachedFilesUrlPrefix: " + saveOptions.AttachedFilesUrlPrefix);
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


