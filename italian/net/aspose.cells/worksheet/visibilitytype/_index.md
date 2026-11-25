---
title: "Worksheet.VisibilityType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Indica lo stato di visibilità di questo foglio"
type: docs
url: /it/net/aspose.cells/worksheet/visibilitytype/
---
## Worksheet.VisibilityType property

Indica lo stato di visibilità per questo foglio.

```csharp
public VisibilityType VisibilityType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyVisibilityTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi fogli di lavoro
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Imposta diversi tipi di visibilità per ogni foglio di lavoro
            workbook.Worksheets[0].VisibilityType = VisibilityType.Hidden;
            workbook.Worksheets[1].VisibilityType = VisibilityType.VeryHidden;
            workbook.Worksheets[2].VisibilityType = VisibilityType.Visible;

            // Salva la cartella di lavoro
            string outputPath = "output_visibility.xlsx";
            workbook.Save(outputPath);

            // Ricarica la cartella di lavoro per verificare le impostazioni di visibilità
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Mostra i tipi di visibilità
            Console.WriteLine("Worksheet 0 Visibility: " + loadedWorkbook.Worksheets[0].VisibilityType);
            Console.WriteLine("Worksheet 1 Visibility: " + loadedWorkbook.Worksheets[1].VisibilityType);
            Console.WriteLine("Worksheet 2 Visibility: " + loadedWorkbook.Worksheets[2].VisibilityType);
        }
    }
}
```

### Vedi anche

* enum [VisibilityType](../../visibilitytype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


