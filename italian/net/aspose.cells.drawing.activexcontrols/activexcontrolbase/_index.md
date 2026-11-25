---
title: "Classe ActiveXControlBase"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ActiveXControlBase class. Rappresenta il controllo ActiveX"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/
---
## ActiveXControlBase class

Rappresenta il controllo ActiveX.

```csharp
public abstract class ActiveXControlBase
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Ottiene e imposta il colore ole dello sfondo. |
| virtual [Data](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/data/) { get; } | Ottiene e imposta i dati binari del controllo. |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Ottiene e imposta il colore OLE del primo piano. |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Ottiene e imposta l'altezza del controllo in unità di punti. |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indica se questo controllo è visibile. |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Ottiene e imposta la cella collegata. |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Ottiene e imposta l'intervallo di riempimento dell'elenco. |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Ottiene e imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo. |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Ottiene e imposta il tipo di icona visualizzata come puntatore del mouse per il controllo. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indica se mostrare un'ombra. |
| abstract [Type](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/type/) { get; } | Ottiene il tipo del controllo ActiveX. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Ottiene e imposta la larghezza del controllo in unità di punti. |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Ottiene l'oggetto [`Workbook`](./workbook/). |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlBaseDemo
    {
        public static void ActiveXControlBaseExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 100, 20);

            CheckBoxActiveXControl control = (CheckBoxActiveXControl)shape.ActiveXControl;
            control.Font.Size = 20;

            // Imposta le proprietà del controllo ActiveX
            control.Width = 150;
            control.Height = 30;
            control.MousePointer = ControlMousePointerType.Arrow;
            control.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Red);
            control.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Yellow);
            control.IsVisible = true;
            control.Shadow = true;
            control.LinkedCell = "A1";
            control.ListFillRange = "A2:A10";

            // Salva la cartella di lavoro
            workbook.Save("ActiveXControlBaseExample.xlsx");
            workbook.Save("ActiveXControlBaseExample.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


