---
title: "HtmlSaveOptions.AttachedFilesDirectory"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Le répertoire où les fichiers joints seront enregistrés. Seulement pour l'enregistrement vers un flux html."
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/attachedfilesdirectory/
---
## HtmlSaveOptions.AttachedFilesDirectory property

Le répertoire où les fichiers joints seront enregistrés. Uniquement pour l'enregistrement dans un flux html.

```csharp
public string AttachedFilesDirectory { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAttachedFilesDirectoryDemo
    {
        public static void Run()
        {
            // Créer un répertoire temporaire pour la démonstration.
            string tempDir = Path.Combine(Path.GetTempPath(), "AsposeAttachedFilesDemo");
            Directory.CreateDirectory(tempDir);

            try
            {
                // Créer un classeur d'exemple
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue("Hello World");

                // Définir les options d'enregistrement HTML avec AttachedFilesDirectory.
                HtmlSaveOptions options = new HtmlSaveOptions();
                options.AttachedFilesDirectory = tempDir;

                // Enregistrez le classeur au format HTML
                string outputPath = Path.Combine(tempDir, "output.html");
                workbook.Save(outputPath, options);

                // Vérifier que les fichiers joints ont été créés.
                Console.WriteLine("HTML saved with attached files in: " + tempDir);
                Console.WriteLine("Attached files exist: " + 
                    File.Exists(Path.Combine(tempDir, "sheet001.htm")));
            }
            finally
            {
                // Nettoyer
                Directory.Delete(tempDir, true);
            }
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


