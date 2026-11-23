---
title: "HtmlSaveOptions.ExportPageHeaders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si l'exportation des en-têtes de page"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportpageheaders/
---
## HtmlSaveOptions.ExportPageHeaders property

Indique si l'exportation des en-têtes de page est activée.

```csharp
public bool ExportPageHeaders { get; set; }
```

### Remarques

Fonctionne uniquement lorsque [`SaveAsSingleFile`](../saveassinglefile/) est vrai.

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageHeadersDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir l’en-tête de page
            worksheet.PageSetup.SetHeader(0, "Sample Header Text");
            
            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue("This is a test");
            
            // Configurer les options d'enregistrement HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                SaveAsSingleFile = true,
                ShowAllSheets = true,
                ExportPageHeaders = true  // This is the key property being demonstrated
            };
            
            // Enregistrez le classeur au format HTML
            string outputPath = "output_with_headers.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file with page headers exported successfully.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


