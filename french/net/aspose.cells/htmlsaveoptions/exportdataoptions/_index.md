---
title: "HtmlSaveOptions.ExportDataOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique la règle d'exportation des données du fichier HTML. La valeur par défaut est All"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportdataoptions/
---
## HtmlSaveOptions.ExportDataOptions property

Indiquant la règle d'exportation des données du fichier html. La valeur par défaut est All.

```csharp
public HtmlExportDataOptions ExportDataOptions { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportDataOptionsDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec des données de test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Créer des options d'enregistrement HTML et définir ExportDataOptions
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
            htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;

            // Enregistrer en HTML avec toutes les options d'exportation de données
            workbook.Save("output.html", htmlSaveOptions);

            Console.WriteLine("HTML file saved with ExportDataOptions.All");
        }
    }
}
```

### Voir aussi

* enum [HtmlExportDataOptions](../../htmlexportdataoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


