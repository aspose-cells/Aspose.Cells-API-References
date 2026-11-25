---
title: "Classe UnknownControl"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.UnknownControl class. Controllo sconosciuto"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/unknowncontrol/
---
## UnknownControl class

Controllo sconosciuto.

```csharp
public class UnknownControl : ActiveXControl
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Ottiene e imposta il colore ole dello sfondo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/unknowncontrol/data/) { get; } | Ottiene e imposta i dati binari del controllo. |
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
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Ottiene e imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Ottiene e imposta il tipo di icona visualizzata come puntatore del mouse per il controllo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indica se mostrare un'ombra.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Rappresenta come allineare il testo usato dal controllo.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/unknowncontrol/type/) { get; } | Ottiene il tipo del controllo ActiveX. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Ottiene e imposta la larghezza del controllo in unità di punti.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Ottiene l'oggetto [`Workbook`](../activexcontrolbase/workbook/).(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetRelationshipData](../../aspose.cells.drawing.activexcontrols/unknowncontrol/getrelationshipdata/)(string) | Ottiene i dati correlati. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlsClassUnknownControlDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo Unknown ActiveX al foglio di lavoro
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Unknown,
                0,  // topRow
                0,  // top
                0,  // leftColumn
                0,  // left
                100,// width
                50  // height
            );

            // Ottieni l'istanza UnknownControl dalla forma
            UnknownControl unknownControl = (UnknownControl)shape.ActiveXControl;
            unknownControl.IsVisible = true;

            // Salva la cartella di lavoro
            workbook.Save("UnknownControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


