---
title: "HtmlSaveOptions.IsExportComments"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HtmlSaveOptions. Indique si l'exportation des commentaires lors de l'enregistrement du fichier en HTML est activée. La valeur par défaut est false"
type: docs
url: /fr/net/aspose.cells/htmlsaveoptions/isexportcomments/
---
## HtmlSaveOptions.IsExportComments property

Indique s’il faut exporter les commentaires lors de l’enregistrement du fichier en HTML, la valeur par défaut est false.

```csharp
public bool IsExportComments { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsExportCommentsDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des données d'exemple et des commentaires
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Ajouter un commentaire
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";
            
            // Enregistrer avec IsExportComments = false (les commentaires ne seront pas exportés)
            HtmlSaveOptions options1 = new HtmlSaveOptions
            {
                IsExportComments = false
            };
            workbook.Save("output_without_comments.html", options1);
            
            // Enregistrer avec IsExportComments = true (les commentaires seront exportés)
            HtmlSaveOptions options2 = new HtmlSaveOptions
            {
                IsExportComments = true
            };
            workbook.Save("output_with_comments.html", options2);
            
            Console.WriteLine("HTML files created successfully.");
        }
    }
}
```

### Voir aussi

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


