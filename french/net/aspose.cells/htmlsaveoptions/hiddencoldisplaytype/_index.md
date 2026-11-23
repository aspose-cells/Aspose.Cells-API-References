---
title: "HtmlSaveOptions.HiddenColDisplayType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Colonne masquée : la largeur de cette colonne est 0 dans Excel. Avant d’enregistrer ce classeur au format HTML, si HtmlHiddenColDisplayType est Removethe, la colonne masquée ne sera pas exportée ; si la valeur est Hidden, la colonne sera exportée mais masquée. La valeur par défaut est Hidden"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/hiddencoldisplaytype/
---
## HtmlSaveOptions.HiddenColDisplayType property

Colonne masquée (la largeur de cette colonne est 0) dans excel, avant de l'enregistrer au format html, si HtmlHiddenColDisplayType est "Remove", la colonne masquée ne sera pas sortie, si la valeur est "Hidden", la colonne sera sortie mais restera masquée, la valeur par défaut est "Hidden"

```csharp
public HtmlHiddenColDisplayType HiddenColDisplayType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenColDisplayTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Masquez la colonne C (index 2)
            worksheet.Cells.HideColumn(2);

            // Ajouter des données pour démontrer
            worksheet.Cells["A1"].PutValue("Visible Column A");
            worksheet.Cells["B1"].PutValue("Visible Column B");
            worksheet.Cells["C1"].PutValue("Hidden Column C");
            worksheet.Cells["D1"].PutValue("Visible Column D");

            // Créez des options d'enregistrement HTML avec différents paramètres HiddenColDisplayType
            HtmlSaveOptions optionsRemove = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Remove
            };

            HtmlSaveOptions optionsHidden = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden
            };

            // Enregistrez avec différentes options
            workbook.Save("output_remove.html", optionsRemove); // Column C will be removed
            workbook.Save("output_hidden.html", optionsHidden); // Column C will be hidden but space preserved
        }
    }
}
```

### Voir aussi

* enum [HtmlHiddenColDisplayType](../../htmlhiddencoldisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


