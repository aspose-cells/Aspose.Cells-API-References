---
title: "MsoLineFormat.Weight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MsoLineFormat. Restituisce o imposta lo spessore della linea in unità di pt"
type: docs
url: /it/net/aspose.cells.drawing/msolineformat/weight/
---
## MsoLineFormat.Weight property

Restituisce o imposta lo spessore della linea, in unità di pt.

```csharp
public double Weight { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyWeightDemo
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
            
            // Accedi al formato linea della forma del commento e imposta lo spessore
            comment.CommentShape.LineFormat.Weight = 0.75;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Verifica che lo spessore sia stato impostato correttamente
            Console.WriteLine("Line weight: " + worksheet.Comments[0].CommentShape.LineFormat.Weight);
        }
    }
}
```

### Vedi anche

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


