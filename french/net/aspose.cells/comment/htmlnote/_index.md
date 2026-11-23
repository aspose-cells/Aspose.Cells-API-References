---
title: "Comment.HtmlNote"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Comment. Obtient et définit la chaîne html qui contient des données et certains formats dans ce commentaire"
type: docs
url: /fr/net/aspose.cells/comment/htmlnote/
---
## Comment.HtmlNote property

Obtient et définit la chaîne HTML qui contient les données et certains formats dans ce commentaire.

```csharp
public string HtmlNote { get; set; }
```

### Remarques

Si c'est un commentaire en fil, la note ne peut pas être modifiée, sinon MS Excel ne pourrait pas le traiter comme un commentaire en fil.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHtmlNoteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            comment.HtmlNote = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            
            workbook.Save("CommentHtmlNoteDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


