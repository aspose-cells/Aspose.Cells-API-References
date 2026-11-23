---
title: "HtmlSaveOptions.ExportActiveWorksheetOnly"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si l'exportation ne concerne que la feuille de calcul active vers un fichier html. Si vrai, alors seule la feuille de calcul active sera exportée vers le fichier html. Si faux, alors l'ensemble du classeur sera exporté vers le fichier html. La valeur par défaut est false."
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportactiveworksheetonly/
---
## HtmlSaveOptions.ExportActiveWorksheetOnly property

Indique s'il faut n'exporter que la feuille de calcul active en fichier html. Si true, alors seule la feuille active sera exportée en html ; si false, tout le classeur sera exporté en html. La valeur par défaut est false.

```csharp
public bool ExportActiveWorksheetOnly { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportActiveWorksheetOnlyDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec deux feuilles de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Ajouter des données d'exemple aux deux feuilles
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Définir les options d'enregistrement HTML pour n'exporter que la feuille de calcul active
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            
            // Définir la première feuille de calcul comme active
            workbook.Worksheets.ActiveSheetIndex = 0;
            
            // Enregistrer en n'incluant que la feuille de calcul active
            workbook.Save("output_active_sheet_only.html", saveOptions);
            
            // Changer la feuille active et enregistrer à nouveau
            workbook.Worksheets.ActiveSheetIndex = 1;
            workbook.Save("output_active_sheet_only2.html", saveOptions);
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


