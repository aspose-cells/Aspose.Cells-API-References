---
title: "SaveOptions.SaveFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SaveOptions. Obtient le format du fichier enregistré"
type: docs
url: /fr/net/aspose.cells/saveoptions/saveformat/
---
## SaveOptions.SaveFormat property

Obtient le format du fichier d'enregistrement.

```csharp
public SaveFormat SaveFormat { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");

            // Démontrer différents formats d'enregistrement
            SaveOptions[] options = {
                new PdfSaveOptions(),
                new OoxmlSaveOptions(),
                new HtmlSaveOptions()
            };

            foreach (var saveOptions in options)
            {
                string extension = FileFormatUtil.SaveFormatToExtension(saveOptions.SaveFormat);
                Console.WriteLine($"Saving as {saveOptions.SaveFormat} with extension: {extension}");

                string outputPath = $"output_{Guid.NewGuid().ToString("N").Substring(0, 8)}{extension}";
                workbook.Save(outputPath, saveOptions);
                Console.WriteLine($"Saved to: {outputPath}");
            }

            // Nettoyer
            workbook.Dispose();
        }
    }
}
```

### Voir aussi

* enum [SaveFormat](../../saveformat/)
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


