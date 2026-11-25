---
title: "Classe SpinButtonActiveXControl"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl class. Rappresenta il controllo SpinButton"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/
---
## SpinButtonActiveXControl class

Rappresenta il controllo SpinButton.

```csharp
public class SpinButtonActiveXControl : ActiveXControl
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Ottiene e imposta il colore ole dello sfondo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Ottiene e imposta i dati binari del controllo.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Rappresenta il carattere del controllo.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Ottiene e imposta il colore ole del primo piano.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Ottiene e imposta l'altezza del controllo in unità di punti.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Ottiene e imposta la modalità di esecuzione predefinita dell'Input Method Editor per il controllo quando riceve il focus.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Indica se i dati nel controllo sono bloccati per la modifica.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Indica se il controllo è trasparente.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indica se questo controllo è visibile.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Ottiene e imposta la cella collegata.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Ottiene e imposta l'intervallo di riempimento dell'elenco.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Max](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max/) { get; set; } | Ottiene e imposta il valore massimo accettabile. |
| [Min](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min/) { get; set; } | Ottiene e imposta il valore minimo accettabile. |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Ottiene e imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Ottiene e imposta il tipo di icona visualizzata come puntatore del mouse per il controllo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Orientation](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation/) { get; set; } | Ottiene e imposta se lo SpinButton o lo ScrollBar è orientato verticalmente o orizzontalmente. |
| [Position](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position/) { get; set; } | Ottiene e imposta il valore. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indica se mostrare un'ombra.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [SmallChange](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/smallchange/) { get; set; } | Ottiene e imposta la quantità di variazione della proprietà Position |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Rappresenta come allineare il testo usato dal controllo.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type/) { get; } | Ottiene il tipo del controllo ActiveX. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Ottiene e imposta la larghezza del controllo in unità di punti.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Ottiene l'oggetto [`Workbook`](../activexcontrolbase/workbook/).(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class SpinButtonActiveXControlDemo
    {
        public static void SpinButtonActiveXControlExample()
        {
            // Inizializza una nuova cartella di lavoro.
            Workbook workbook = new Workbook();

            // Aggiungi un SpinButtonActiveXControl.
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.SpinButton, 1, 0, 1, 0, 100, 50);
            SpinButtonActiveXControl activeXControl = (SpinButtonActiveXControl)shape.ActiveXControl;

            // Impostazione delle proprietà
            activeXControl.Min = 0;
            activeXControl.Max = 100;
            activeXControl.Position = 30;
            activeXControl.SmallChange = 5;

            if (activeXControl.Orientation == ControlScrollOrientation.Auto)
            {
                activeXControl.Orientation = ControlScrollOrientation.Horizontal;
            }

            activeXControl.IsEnabled = true;
            activeXControl.IsLocked = false;
            activeXControl.IsTransparent = false;
            activeXControl.IsAutoSize = true;
            activeXControl.IMEMode = InputMethodEditorMode.On;
            activeXControl.TextAlign = TextAlignmentType.Center;
            activeXControl.Width = 150;
            activeXControl.Height = 30;
            activeXControl.MousePointer = ControlMousePointerType.Default;
            activeXControl.ForeOleColor = 0x000000; // Black color
            activeXControl.BackOleColor = 0xFFFFFF; // White color
            activeXControl.IsVisible = true;
            activeXControl.Shadow = false;
            activeXControl.LinkedCell = "A1";
            activeXControl.ListFillRange = "A2:A10";

            // Salva la cartella di lavoro
            workbook.Save("SpinButtonActiveXControlExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


