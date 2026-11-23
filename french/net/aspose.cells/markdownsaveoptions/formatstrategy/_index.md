---
title: "MarkdownSaveOptions.FormatStrategy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété MarkdownSaveOptions. Obtient et définit la stratégie de format lors de l'exportation de la valeur de la cellule en tant que chaîne"
type: docs
url: /fr/net/aspose.cells/markdownsaveoptions/formatstrategy/
---
## MarkdownSaveOptions.FormatStrategy property

Obtient et définit la stratégie de format lors de l'exportation de la valeur de la cellule en tant que chaîne.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple avec différents formats
            worksheet.Cells["A1"].PutValue(123.456); // Numeric value
            worksheet.Cells["A2"].PutValue(DateTime.Now); // Date value
            worksheet.Cells["A3"].PutValue(true); // Boolean value

            // Créez des options d'enregistrement Markdown avec la stratégie de format DisplayString
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayString
            };

            // Enregistrez le classeur au format Markdown
            workbook.Save("MarkdownWithDisplayString.md", saveOptions);

            // Passez à CellValueFormatStrategy.CellStyle
            saveOptions.FormatStrategy = CellValueFormatStrategy.CellStyle;
            workbook.Save("MarkdownWithCellStyle.md", saveOptions);

            Console.WriteLine("Markdown files saved successfully with different format strategies.");
        }
    }
}
```

### Voir aussi

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


