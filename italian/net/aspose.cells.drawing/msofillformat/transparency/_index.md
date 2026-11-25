---
title: "MsoFillFormat.Transparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoFillFormat. Restituisce o imposta il grado di trasparenza del riempimento specificato come valore da 0,0 opaco a 1,0 trasparente"
type: docs
url: /it/net/aspose.cells.drawing/msofillformat/transparency/
---
## MsoFillFormat.Transparency property

Restituisce o imposta il grado di trasparenza del riempimento specificato come valore da 0.0 (opaco) a 1.0 (trasparente).

```csharp
public double Transparency { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Imposta le proprietà del formato di riempimento includendo la trasparenza
            comment.CommentShape.FillFormat.IsVisible = true;
            comment.CommentShape.FillFormat.ForeColor = System.Drawing.Color.Red;
            comment.CommentShape.FillFormat.BackColor = System.Drawing.Color.Yellow;
            
            // Imposta la trasparenza (0,0 = completamente opaco, 1,0 = completamente trasparente)
            comment.CommentShape.FillFormat.Transparency = 0.5;

            // Salva la cartella di lavoro
            workbook.Save("CommentTransparencyDemo.xlsx");

            // Carica la cartella di lavoro salvata per verificare la trasparenza
            Workbook verifyWorkbook = new Workbook("CommentTransparencyDemo.xlsx");
            Comment verifyComment = verifyWorkbook.Worksheets[0].Comments[0];
            
            // Emetti il valore della trasparenza per dimostrare che è stato salvato e caricato correttamente
            Console.WriteLine("Comment fill transparency: " + 
                verifyComment.CommentShape.FillFormat.Transparency);
        }
    }
}
```

### Vedi anche

* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


