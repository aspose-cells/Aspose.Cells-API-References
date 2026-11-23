---
title: "HtmlSaveOptions.HiddenRowDisplayType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Ligne masquée : la hauteur de cette ligne est 0 dans Excel avant de l'enregistrer au format HTML. Si HtmlHiddenRowDisplayType est Remove, la ligne masquée ne sera pas sortie. Si la valeur est Hidden, la ligne sera sortie mais masquée. La valeur par défaut est Hidden"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/
---
## HtmlSaveOptions.HiddenRowDisplayType property

Ligne masquée (la hauteur de cette ligne est 0) dans Excel, avant de l’enregistrer au format HTML, si HtmlHiddenRowDisplayType est "Remove", la ligne masquée ne sera pas sortie, si la valeur est "Hidden", la ligne sera sortie mais masquée, la valeur par défaut est "Hidden"

```csharp
public HtmlHiddenRowDisplayType HiddenRowDisplayType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenRowDisplayTypeDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple et masquer une ligne
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row");
            worksheet.Cells.HideRow(1); // Hide row 2 (0-based index 1)

            // Définir les options d'enregistrement HTML avec HiddenRowDisplayType
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;

            // Enregistrer au format HTML
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with hidden rows handled according to HiddenRowDisplayType setting.");
        }
    }
}
```

### Voir aussi

* enum [HtmlHiddenRowDisplayType](../../htmlhiddenrowdisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


