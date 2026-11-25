---
title: "PaneCollection.FirstVisibleColumnOfRightPane"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaneCollection. Ottiene e imposta la prima colonna visibile del riquadro destro"
type: docs
url: /it/net/aspose.cells/panecollection/firstvisiblecolumnofrightpane/
---
## PaneCollection.FirstVisibleColumnOfRightPane property

Ottiene e imposta la prima colonna visibile del riquadro destro.

```csharp
public int FirstVisibleColumnOfRightPane { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleColumnOfRightPaneDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Blocca i riquadri specificando gli indici di riga e colonna (5, 3)
            sheet.FreezePanes(5, 3, 5, 3);
            
            // Ottieni la collezione dei riquadri
            PaneCollection panes = sheet.GetPanes();
            
            // Imposta la prima colonna visibile del riquadro destro
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


