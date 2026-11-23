---
title: "Énumération HtmlExportDataOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.HtmlExportDataOptions. Représente les options d'exportation des données html"
type: docs
url: /fr/net/aspose.cells/htmlexportdataoptions/
---
## HtmlExportDataOptions enumeration

Représente les options d'exportation des données HTML.

```csharp
public enum HtmlExportDataOptions
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Table | `1` | Exporter le fichier en html contenant uniquement la partie tableau. |
| All | `255` | Exporter toutes les données en html. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlExportDataOptionsDemo
    {
        public static void HtmlExportDataOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane Doe");
            worksheet.Cells["B3"].PutValue(25);

            // Créer HtmlSaveOptions et définir le HtmlExportDataOptions
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportDataOptions = HtmlExportDataOptions.All; // Export all data to HTML

            // Enregistrer le classeur au format HTML
            workbook.Save("HtmlExportDataOptionsExample_All.html", saveOptions);

            // Modifier le HtmlExportDataOptions pour n'exporter que la partie tableau
            saveOptions.ExportDataOptions = HtmlExportDataOptions.Table; // Export only the table part

            // Enregistrer à nouveau le classeur au format HTML
            workbook.Save("HtmlExportDataOptionsExample_Table.html", saveOptions);

            Console.WriteLine("HTML files have been saved successfully.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


