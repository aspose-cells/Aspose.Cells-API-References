---
title: "HtmlSaveOptions.ExportHiddenWorksheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si le contenu de la feuille de calcul masquée est exporté. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exporthiddenworksheet/
---
## HtmlSaveOptions.ExportHiddenWorksheet property

Indiquant si l'exportation du contenu de la feuille de calcul masquée est activée. La valeur par défaut est true.

```csharp
public bool ExportHiddenWorksheet { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportHiddenWorksheetDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "VisibleSheet";
            worksheet1.Cells["A1"].PutValue("Visible Data");

            Worksheet worksheet2 = workbook.Worksheets.Add("HiddenSheet");
            worksheet2.Cells["A1"].PutValue("Hidden Data");
            worksheet2.IsVisible = false;

            // Définissez les options d'enregistrement HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportHiddenWorksheet = false, // Don't export hidden worksheets
                ExportActiveWorksheetOnly = false
            };

            // Enregistrer avec la feuille masquée non exportée
            workbook.Save("output_without_hidden.html", saveOptions);

            // Modifier l'option pour exporter les feuilles masquées
            saveOptions.ExportHiddenWorksheet = true;

            // Enregistrer avec la feuille masquée exportée
            workbook.Save("output_with_hidden.html", saveOptions);
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


