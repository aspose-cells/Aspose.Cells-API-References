---
title: "Comment.HeightCM"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Rappresenta l'altezza del commento in unità di centimetri"
type: docs
url: /it/net/aspose.cells/comment/heightcm/
---
## Comment.HeightCM property

Rappresenta l'altezza del commento, in unità di centimetri.

```csharp
public double HeightCM { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightCMDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Imposta il testo del commento
            comment.Note = "Sample comment";
            
            // Imposta l'altezza del commento in centimetri
            comment.HeightCM = 1.5;
            
            // Salva la cartella di lavoro
            workbook.Save("CommentHeightCMDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


