---
title: "MarkdownSaveOptions.MarkdownSaveOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur MarkdownSaveOptions. Crée des options pour enregistrer un document markdown"
type: docs
url: /fr/net/aspose.cells/markdownsaveoptions/markdownsaveoptions/
---
## MarkdownSaveOptions constructor

Crée des options pour enregistrer le document markdown

```csharp
public MarkdownSaveOptions()
```

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Démontrez le constructeur MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                LineSeparator = Environment.NewLine
            };

            // Enregistrer au format Markdown
            workbook.Save("MarkdownOutput.md", saveOptions);

            Console.WriteLine("Markdown file created successfully.");
        }
    }
}
```

### Voir aussi

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


