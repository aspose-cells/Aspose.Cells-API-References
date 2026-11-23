---
title: "HtmlSaveOptions.FormatDataIgnoreColumnWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique s'il faut afficher toutes les données formatées d'une cellule lorsqu'elle dépasse la colonne. Si true, la largeur de colonne est ignorée et toutes les données de la cellule seront exportées. Si false, les données seront exportées comme dans Excel. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/
---
## HtmlSaveOptions.FormatDataIgnoreColumnWidth property

Indiquant si l'affichage de l'intégralité des données formatées d'une cellule est activé lorsqu'elle dépasse la largeur de la colonne. Si true, la largeur de la colonne est ignorée et toutes les données de la cellule seront exportées. Si false, les données seront exportées comme dans Excel. La valeur par défaut est false.

```csharp
public bool FormatDataIgnoreColumnWidth { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFormatDataIgnoreColumnWidthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir des données d'exemple et la largeur de colonne
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B1"].PutValue("Longer Text That Might Be Truncated");
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 5);  // Very narrow column

            // Créer des options d'enregistrement HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Démontrer la propriété FormatDataIgnoreColumnWidth
            saveOptions.FormatDataIgnoreColumnWidth = true; // Text won't be truncated by column width
            
            // Enregistrer avec différents paramètres pour montrer l'effet
            workbook.Save("HtmlWithIgnoreColumnWidth.html", saveOptions);
            
            saveOptions.FormatDataIgnoreColumnWidth = false; // Text may be truncated by column width
            workbook.Save("HtmlWithoutIgnoreColumnWidth.html", saveOptions);
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


