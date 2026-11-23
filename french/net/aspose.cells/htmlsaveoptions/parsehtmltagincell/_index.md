---
title: "HtmlSaveOptions.ParseHtmlTagInCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si les balises html telles que div/div dans la cellule doivent être analysées comme valeur de cellule ou conservées telles quelles. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/parsehtmltagincell/
---
## HtmlSaveOptions.ParseHtmlTagInCell property

Indique si les balises HTML (comme `<div></div>`) dans une cellule doivent être analysées comme valeur de cellule ou conservées telles quelles. La valeur par défaut est true.

```csharp
public bool ParseHtmlTagInCell { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyParseHtmlTagInCellDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des données d'exemple contenant des balises HTML
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir la valeur de la cellule avec des balises HTML
            worksheet.Cells["A1"].PutValue("<b>Bold Text</b> and <i>Italic Text</i>");
            
            // Créer des options d'enregistrement HTML et activer l'analyse des balises HTML
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html);
            htmlSaveOptions.ParseHtmlTagInCell = true;
            
            // Enregistrer le classeur avec les balises HTML analysées
            workbook.Save("output.html", htmlSaveOptions);
            
            Console.WriteLine("HTML saved with ParseHtmlTagInCell enabled.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


