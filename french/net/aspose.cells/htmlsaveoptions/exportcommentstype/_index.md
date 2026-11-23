---
title: "HtmlSaveOptions.ExportCommentsType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Représente le type d'exportation des commentaires vers des fichiers html."
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/exportcommentstype/
---
## HtmlSaveOptions.ExportCommentsType property

Représente le type d'exportation des commentaires vers les fichiers html.

```csharp
public PrintCommentsType ExportCommentsType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCommentsTypeDemo
    {
        public static void Run()
        {
            // Créez un classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un commentaire d'exemple en utilisant le nom de la cellule.
            Comment comment = worksheet.Comments["A1"];
            comment.Note = "This is a test comment";
            
            // Définir les options d'enregistrement HTML avec ExportCommentsType.
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportCommentsType = PrintCommentsType.PrintInPlace;
            
            // Enregistrer au format HTML
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file with comments exported successfully.");
        }
    }
}
```

### Voir aussi

* enum [PrintCommentsType](../../printcommentstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


