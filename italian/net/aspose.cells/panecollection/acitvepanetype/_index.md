---
title: "PaneCollection.AcitvePaneType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaneCollection. Ottiene e imposta il riquadro attivo"
type: docs
url: /it/net/aspose.cells/panecollection/acitvepanetype/
---
## PaneCollection.AcitvePaneType property

Ottiene e imposta il riquadro attivo.

```csharp
[Obsolete("Use PaneCollection.ActivePaneType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public RectangleAlignmentType AcitvePaneType { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà [`ActivePaneType`](../activepanetype/). Questo metodo sarà rimosso 12 mesi dopo, a partire da luglio 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PaneCollectionPropertyAcitvePaneTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per dimostrare la divisione dei riquadri
            for (int i = 0; i < 20; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i + 1}, Col {j + 1}";
                }
            }

            // Dividi il foglio di lavoro in riquadri
            worksheet.Split();

            // Ottieni la collezione dei riquadri
            PaneCollection panes = worksheet.GetPanes();

            // Visualizza il riquadro attivo corrente
            Console.WriteLine("Current ActivePaneType: " + panes.AcitvePaneType);

            // Imposta il riquadro attivo su BottomRight
            panes.AcitvePaneType = RectangleAlignmentType.BottomRight;
            Console.WriteLine("Changed ActivePaneType to: " + panes.AcitvePaneType);

            // Imposta la prima riga/colonna visibile per i riquadri inferiore/destro
            panes.FirstVisibleRowOfBottomPane = 15;
            panes.FirstVisibleColumnOfRightPane = 7;

            // Salva la cartella di lavoro
            workbook.Save("PaneCollectionActivePaneTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [RectangleAlignmentType](../../../aspose.cells.drawing/rectanglealignmenttype/)
* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


