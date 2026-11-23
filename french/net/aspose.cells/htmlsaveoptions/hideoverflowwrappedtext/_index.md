---
title: "HtmlSaveOptions.HideOverflowWrappedText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique s’il faut masquer le texte débordant lorsque le format de la cellule est défini sur le renvoi à la ligne. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/hideoverflowwrappedtext/
---
## HtmlSaveOptions.HideOverflowWrappedText property

Indique s’il faut masquer le texte débordant lorsque le format de la cellule est défini sur retour à la ligne. La valeur par défaut est false

```csharp
public bool HideOverflowWrappedText { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHideOverflowWrappedTextDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez le texte d’exemple dans la cellule A1
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap and hide overflow when exported to HTML");
            
            // Créez et appliquez un style avec le renvoi à la ligne du texte
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;
            
            // Obtenez la collection de cellules et appliquez le style
            Cells cells = worksheet.Cells;
            cells["A1"].SetStyle(style, flag);
            
            // Définissez la largeur de colonne pour que le texte se renvoie à la ligne
            cells.SetColumnWidth(0, 10);
            
            // Créez les options d’enregistrement HTML et définissez HideOverflowWrappedText
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.HideOverflowWrappedText = true;
            
            // Enregistrer le classeur avec les options HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("File saved with HideOverflowWrappedText: " + outputPath);
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


