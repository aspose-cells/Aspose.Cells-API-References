---
title: "Classe CommandButtonActiveXControl"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Drawing.ActiveXControls.CommandButtonActiveXControl. Rappresenta un pulsante di comando"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/
---
## CommandButtonActiveXControl class

Rappresenta un pulsante di comando.

```csharp
public class CommandButtonActiveXControl : ActiveXControl
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Accelerator](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/accelerator/) { get; set; } | Ottiene e imposta il tasto di accelerazione per il controllo. |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Ottiene e imposta il colore ole dello sfondo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Caption](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/caption/) { get; set; } | Ottiene e imposta il testo descrittivo che appare su un controllo. |
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
| [IsWordWrapped](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/iswordwrapped/) { get; set; } | Indica se il contenuto del controllo va a capo automaticamente alla fine di una riga. |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Ottiene e imposta la cella collegata.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Ottiene e imposta l'intervallo di riempimento dell'elenco.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Ottiene e imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Ottiene e imposta il tipo di icona visualizzata come puntatore del mouse per il controllo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Picture](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/picture/) { get; set; } | Ottiene e imposta i dati dell'immagine. |
| [PicturePosition](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/pictureposition/) { get; set; } | Ottiene e imposta la posizione dell'immagine del controllo rispetto alla sua didascalia. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indica se mostrare un'ombra.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TakeFocusOnClick](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/takefocusonclick/) { get; set; } | Indica se il controllo prende il focus quando viene cliccato. |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Rappresenta come allineare il testo usato dal controllo.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/type/) { get; } | Ottiene il tipo del controllo ActiveX. |
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

    public class CommandButtonActiveXControlDemo
    {
        public static void CommandButtonActiveXControlExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX CommandButton al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2,2,2, 100, 30);
            CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà del controllo ActiveX CommandButton
            commandButton.Caption = "Click Me";
            commandButton.PicturePosition = ControlPicturePositionType.Center;
            commandButton.Accelerator = 'C';
            commandButton.TakeFocusOnClick = true;
            commandButton.IsWordWrapped = true;
            commandButton.IsEnabled = true;
            commandButton.IsLocked = false;
            commandButton.IsTransparent = false;
            commandButton.IsAutoSize = false;
            commandButton.IMEMode = InputMethodEditorMode.NoControl;
            commandButton.TextAlign = TextAlignmentType.Center;
            commandButton.Width = 150;
            commandButton.Height = 50;
            commandButton.MousePointer = ControlMousePointerType.Default;
            commandButton.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
            commandButton.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
            commandButton.IsVisible = true;
            commandButton.Shadow = true;
            commandButton.LinkedCell = "A1";
            commandButton.ListFillRange = "A2:A10";

            // Salva la cartella di lavoro
            workbook.Save("CommandButtonActiveXControlExample.xlsx");
            workbook.Save("CommandButtonActiveXControlExample.pdf");
        }
    }
}
```

### Vedi anche

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


