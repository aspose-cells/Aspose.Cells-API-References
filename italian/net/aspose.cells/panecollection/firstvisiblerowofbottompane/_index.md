---
title: "PaneCollection.FirstVisibleRowOfBottomPane"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaneCollection. Ottiene e imposta la prima riga visibile del riquadro inferiore"
type: docs
url: /it/net/aspose.cells/panecollection/firstvisiblerowofbottompane/
---
## PaneCollection.FirstVisibleRowOfBottomPane property

Ottiene e imposta la prima riga visibile del riquadro inferiore.

```csharp
public int FirstVisibleRowOfBottomPane { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per creare un riquadro scorrevole
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // Blocca i riquadri alla riga 10 (questo creerà riquadri superiore e inferiore)
            worksheet.FreezePanes(10, 0, 10, 0);
            
            // Ottieni la collezione dei riquadri
            PaneCollection panes = worksheet.GetPanes();
            
            // Imposta la prima riga visibile del riquadro inferiore
            panes.FirstVisibleRowOfBottomPane = 15;
            
            // Restituisci la prima riga visibile del riquadro inferiore
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            
            // Salva la cartella di lavoro
            workbook.Save("PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


