---
title: "HtmlSaveOptions.ExportHeadings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si les en-têtes de lignes et de colonnes des feuilles sont exportés lors de l’enregistrement en fichiers HTML"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportheadings/
---
## HtmlSaveOptions.ExportHeadings property

Indique si l'exportation des en-têtes de lignes et de colonnes de la feuille est activée lors de l'enregistrement en fichiers HTML.

```csharp
[Obsolete("Use HtmlSaveOptions.ExportRowColumnHeadings instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExportHeadings { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété HtmlSaveOptions.ExportRowColumnHeadings. Cette propriété sera supprimée 12 mois après juin 2022. Aspose s’excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportHeadingsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Créer les options d’enregistrement HTML et activer l’exportation des en-têtes
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportHeadings = true;

            // Enregistrer en HTML avec les en-têtes
            workbook.Save("output_with_headings.html", options);
            
            // Enregistrer à nouveau sans les en-têtes pour comparaison
            options.ExportHeadings = false;
            workbook.Save("output_without_headings.html", options);
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


