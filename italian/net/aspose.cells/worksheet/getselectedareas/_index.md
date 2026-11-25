---
title: "Worksheet.GetSelectedAreas"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Ottiene gli intervalli di celle selezionati nel foglio di calcolo del designer"
type: docs
url: /it/net/aspose.cells/worksheet/getselectedareas/
---
## Worksheet.GetSelectedAreas method

Ottiene gli intervalli selezionati di celle nel foglio di calcolo del designer.

```csharp
public Range[] GetSelectedAreas()
```

### Valore di ritorno

Restituisce tutti gli intervalli selezionati.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetSelectedAreasDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Seleziona più intervalli
            worksheet.SelectRange(0, 0, 2, 2, false); // First range (A1:C3)
            worksheet.SelectRange(4, 4, 6, 6, false); // Second range (E5:G7)
            
            // Ottieni le aree selezionate
            Aspose.Cells.Range[] selectedAreas = worksheet.GetSelectedAreas();
            
            // Visualizza le informazioni sulle aree selezionate
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            for (int i = 0; i < selectedAreas.Length; i++)
            {
                Console.WriteLine($"Area {i + 1}: {selectedAreas[i].Address}");
            }
            
            // Cancella le selezioni e seleziona un unico intervallo
            worksheet.SelectRange(1, 1, 3, 3, true); // New single selection (B2:D4)
            
            // Ottieni l'unica area selezionata
            selectedAreas = worksheet.GetSelectedAreas();
            Console.WriteLine("\nAfter single selection:");
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            Console.WriteLine("Selected area: " + selectedAreas[0].Address);
        }
    }
}
```

### Vedi anche

* class [Range](../../range/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


