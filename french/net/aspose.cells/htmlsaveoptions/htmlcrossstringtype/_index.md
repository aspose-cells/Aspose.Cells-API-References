---
title: "HtmlSaveOptions.HtmlCrossStringType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si une chaîne intercellulaire sera affichée de la même manière que MS Excel lors de l'enregistrement d'un fichier Excel au format html. Par défaut, la valeur est Default, ainsi pour les chaînes intercellulaires il y a peu de différence entre les fichiers html créés par Aspose.Cells et MS Excel. Cependant, les performances pour créer de grands fichiers html en définissant la valeur sur Cross seraient plusieurs fois plus rapides que de la définir sur Default ou Fit2Cell."
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/htmlcrossstringtype/
---
## HtmlSaveOptions.HtmlCrossStringType property

Indique si une chaîne traversant plusieurs cellules sera affichée de la même manière que MS Excel lors de l’enregistrement d’un fichier Excel au format HTML. Par défaut, la valeur est Default, ainsi, pour les chaînes traversant plusieurs cellules, il y a peu de différence entre les fichiers HTML créés par Aspose.Cells et MS Excel. Mais les performances pour créer de grands fichiers HTML, en définissant la valeur à Cross, seraient plusieurs fois plus rapides que de la définir à Default ou Fit2Cell.

```csharp
public HtmlCrossType HtmlCrossStringType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHtmlCrossStringTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple qui démontreront le comportement des chaînes intercellulaires
            worksheet.Cells["A1"].PutValue("Left Content");
            worksheet.Cells["B1"].PutValue("Right Content");
            
            // Obtenir et modifier les styles de cellule
            Style styleA1 = worksheet.Cells["A1"].GetStyle();
            styleA1.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["A1"].SetStyle(styleA1);
            
            Style styleB1 = worksheet.Cells["B1"].GetStyle();
            styleB1.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["B1"].SetStyle(styleB1);

            // Configurer les options d'enregistrement HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;

            // Enregistrer le classeur au format HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with CrossHideRight option.");
        }
    }
}
```

### Voir aussi

* enum [HtmlCrossType](../../htmlcrosstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


