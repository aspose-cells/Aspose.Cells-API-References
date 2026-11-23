---
title: "MarkdownSaveOptions.OfficeMathOutputType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MarkdownSaveOptions. Indique comment les objets OfficeMath sont exportés vers Markdown. La valeur par défaut est Image"
type: docs
url: /fr/net/aspose.cells/markdownsaveoptions/officemathoutputtype/
---
## MarkdownSaveOptions.OfficeMathOutputType property

Indique comment les objets OfficeMath sont exportés vers Markdown, la valeur par défaut est Image.

```csharp
public HtmlOfficeMathOutputType OfficeMathOutputType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MarkdownSaveOptionsPropertyOfficeMathOutputTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple incluant une formule qui pourrait contenir OfficeMath
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].Formula = "=SQRT(16)";

            try
            {
                // Créer des options d'enregistrement Markdown
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Afficher la valeur actuelle de OfficeMathOutputType
                Console.WriteLine("Current OfficeMathOutputType: " + saveOptions.OfficeMathOutputType);

                // Définir OfficeMathOutputType sur MathML
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.MathML;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // Enregistrer le classeur avec le type de sortie MathML
                workbook.Save("OfficeMathOutputType_MathML.md", saveOptions);

                // Passer au type de sortie Image
                saveOptions.OfficeMathOutputType = HtmlOfficeMathOutputType.Image;
                Console.WriteLine("Changed OfficeMathOutputType to: " + saveOptions.OfficeMathOutputType);

                // Enregistrer le classeur avec le type de sortie Image
                workbook.Save("OfficeMathOutputType_Image.md", saveOptions);

                Console.WriteLine("OfficeMathOutputType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* enum [HtmlOfficeMathOutputType](../../htmlofficemathoutputtype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


