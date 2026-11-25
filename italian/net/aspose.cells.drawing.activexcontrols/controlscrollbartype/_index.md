---
title: "Enum ControlScrollBarType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType enum. Rappresenta il tipo di barra di scorrimento"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/controlscrollbartype/
---
## ControlScrollBarType enumeration

Rappresenta il tipo di barra di scorrimento.

```csharp
public enum ControlScrollBarType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Non visualizza barre di scorrimento. |
| Horizontal | `1` | Visualizza una barra di scorrimento orizzontale. |
| BarsVertical | `2` | Visualizza una barra di scorrimento verticale. |
| BarsBoth | `3` | Visualizza sia una barra di scorrimento orizzontale sia una verticale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollBarTypeDemo
    {
        public static void ControlScrollBarTypeExample()
        {
            // Inizializza una nuova cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ListBox al foglio di lavoro
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 0, 1, 0, 100, 50);
            ListBoxActiveXControl listBoxControl = (ListBoxActiveXControl)shape.ActiveXControl;

            // Imposta la proprietà ScrollBars per visualizzare sia le barre di scorrimento orizzontali che quelle verticali
            listBoxControl.ScrollBars = ControlScrollBarType.BarsBoth;

            // Salva la cartella di lavoro
            workbook.Save("ControlScrollBarTypeExample.xlsx");
            workbook.Save("ControlScrollBarTypeExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


