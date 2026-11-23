---
title: "HtmlSaveOptions.DisableDownlevelRevealedComments"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si les commentaires conditionnels Downlevelrevealed sont désactivés lors de l'exportation du fichier en html ; la valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/disabledownlevelrevealedcomments/
---
## HtmlSaveOptions.DisableDownlevelRevealedComments property

Indique s'il faut désactiver les commentaires conditionnels Downlevel-revealed lors de l'exportation du fichier en html, la valeur par défaut est false.

```csharp
public bool DisableDownlevelRevealedComments { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDisableDownlevelRevealedCommentsDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec un commentaire
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a test comment";

            // Définir les options d'enregistrement HTML avec DisableDownlevelRevealedComments
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.DisableDownlevelRevealedComments = true;

            // Enregistrer le classeur avec les options HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("Workbook saved with DisableDownlevelRevealedComments=true");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


