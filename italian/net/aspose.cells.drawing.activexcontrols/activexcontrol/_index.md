---
title: "Classe ActiveXControl"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ActiveXControl classe. Rappresenta il controllo ActiveX"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrol/
---
## ActiveXControl class

Rappresenta il controllo ActiveX.

```csharp
public abstract class ActiveXControl : ActiveXControlBase
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Ottiene e imposta il colore ole dello sfondo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Ottiene e imposta i dati binari del controllo. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Rappresenta il font del controllo. |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Ottiene e imposta il colore ole del primo piano.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Ottiene e imposta l'altezza del controllo in unità di punti.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Ottiene e imposta la modalità di esecuzione predefinita dell'Input Method Editor per il controllo quando riceve il focus. |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente. |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Indica se i dati nel controllo sono bloccati per la modifica. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Indica se il controllo è trasparente. |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indica se questo controllo è visibile.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Ottiene e imposta la cella collegata.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Ottiene e imposta l'intervallo di riempimento dell'elenco.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Ottiene e imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Ottiene e imposta il tipo di icona visualizzata come puntatore del mouse per il controllo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indica se mostrare un'ombra.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Rappresenta come allineare il testo utilizzato dal controllo. |
| abstract [Type](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/type/) { get; } | Ottiene il tipo del controllo ActiveX.(Inherited from [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Ottiene e imposta la larghezza del controllo in unità di punti.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Ottiene l'oggetto [`Workbook`](../activexcontrolbase/workbook/).(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassActiveXControlDemo
    {
        public static void Run()
        {
            // Crea cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi il controllo ActiveX RadioButton
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.RadioButton, 
                1, 1,  // upper left row/column
                1, 1,  // upper left row/column offsets
                100, 30);  // width and height
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà
            radioButton.GroupName = "Sheet1";
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            radioButton.IsWordWrapped = true;
            radioButton.Caption = "OptionButton1";
            radioButton.PicturePosition = ControlPicturePositionType.AboveCenter;
            radioButton.SpecialEffect = ControlSpecialEffectType.Sunken;
            radioButton.IsEnabled = true;
            radioButton.IsTransparent = false;
            radioButton.IsAutoSize = false;
            radioButton.IMEMode = InputMethodEditorMode.NoControl;
            radioButton.Font.Name = "Calibri";
            radioButton.MousePointer = ControlMousePointerType.Default;

            // Salva la cartella di lavoro
            workbook.Save("ActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ActiveXControlBase](../activexcontrolbase/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


