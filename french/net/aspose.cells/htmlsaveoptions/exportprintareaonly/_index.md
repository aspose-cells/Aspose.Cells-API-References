---
title: "HtmlSaveOptions.ExportPrintAreaOnly"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si seule la zone d'impression est exportée vers le fichier html. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportprintareaonly/
---
## HtmlSaveOptions.ExportPrintAreaOnly property

Indique si seule la zone d'impression est exportée vers le fichier html. La valeur par défaut est false.

```csharp
public bool ExportPrintAreaOnly { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPrintAreaOnlyDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir des données d'exemple
            for (int i = 0; i < 20; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i+1},{j+1}");
                }
            }

            // Définir la zone d'impression
            worksheet.PageSetup.PrintArea = "B2:F10";

            // Configurer les options d'enregistrement HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportPrintAreaOnly = true;
            options.ExportGridLines = true;

            // Enregistrer le classeur avec uniquement la zone d'impression
            workbook.Save("output.html", options);
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


