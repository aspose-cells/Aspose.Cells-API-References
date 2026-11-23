---
title: "MarkdownSaveOptions.LineSeparator"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MarkdownSaveOptions. Obtient et définit le séparateur de ligne"
type: docs
url: /fr/net/aspose.cells/markdownsaveoptions/lineseparator/
---
## MarkdownSaveOptions.LineSeparator property

Obtient et définit le séparateur de ligne.

```csharp
public string LineSeparator { get; set; }
```

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyLineSeparatorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Value1");
            worksheet.Cells["B2"].PutValue("Value2");

            // Configurer les options d'enregistrement Markdown avec un séparateur de ligne personnalisé
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                LineSeparator = "\n", // Using Unix-style line endings
                Encoding = Encoding.UTF8
            };

            // Enregistrer sous fichier Markdown
            workbook.Save("MarkdownWithLineSeparator.md", saveOptions);

            Console.WriteLine("Markdown file saved with custom line separator.");
        }
    }
}
```

### Voir aussi

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


