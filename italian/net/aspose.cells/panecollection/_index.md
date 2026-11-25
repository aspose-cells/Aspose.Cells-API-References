---
title: "Classe PaneCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.PaneCollection. Rappresenta tutti gli oggetti Pane visualizzati nella finestra specificata"
type: docs
url: /it/net/aspose.cells/panecollection/
---
## PaneCollection class

Rappresenta tutti gli oggetti Pane mostrati nella finestra specificata.

```csharp
public class PaneCollection
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AcitvePaneType](../../aspose.cells/panecollection/acitvepanetype/) { get; set; } | (**Obsoleto.**) Ottiene e imposta il riquadro attivo. |
| [ActivePaneType](../../aspose.cells/panecollection/activepanetype/) { get; set; } | Ottiene e imposta il riquadro attivo. |
| [FirstVisibleColumnOfRightPane](../../aspose.cells/panecollection/firstvisiblecolumnofrightpane/) { get; set; } | Ottiene e imposta la prima colonna visibile del riquadro destro. |
| [FirstVisibleRowOfBottomPane](../../aspose.cells/panecollection/firstvisiblerowofbottompane/) { get; set; } | Ottiene e imposta la prima riga visibile del riquadro inferiore. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPaneCollectionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].Value = $"Row {i}, Col {j}";
                }
            }
            
            // Blocca i riquadri alla riga 5, colonna 1
            sheet.FreezePanes(5, 1, 5, 1);
            
            // Ottieni la collezione di riquadri
            PaneCollection panes = sheet.GetPanes();
            
            // Modifica le impostazioni del riquadro
            panes.FirstVisibleRowOfBottomPane = 5;
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // Salva la cartella di lavoro
            workbook.Save("PaneCollectionDemo.xls", SaveFormat.Excel97To2003);
            
            Console.WriteLine("PaneCollection demo executed successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


