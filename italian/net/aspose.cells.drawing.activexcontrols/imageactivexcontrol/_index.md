---
title: "Classe ImageActiveXControl"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl class. Rappresenta il controllo immagine"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/
---
## ImageActiveXControl class

Rappresenta il controllo immagine.

```csharp
public class ImageActiveXControl : ActiveXControl
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Ottiene e imposta il colore ole dello sfondo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [BorderOleColor](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderolecolor/) { get; set; } | Ottiene e imposta il colore ole dello sfondo. |
| [BorderStyle](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderstyle/) { get; set; } | Ottiene e imposta il tipo di bordo utilizzato dal controllo. |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Ottiene e imposta i dati binari del controllo.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Rappresenta il carattere del controllo.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Ottiene e imposta il colore ole del primo piano.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Ottiene e imposta l'altezza del controllo in unità di punti.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Ottiene e imposta la modalità di esecuzione predefinita dell'Input Method Editor per il controllo quando riceve il focus.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| override [IsAutoSize](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/isautosize/) { get; set; } | Indica se il controllo ridimensionerà automaticamente per visualizzare tutto il contenuto. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Indica se il controllo può ricevere il focus e rispondere agli eventi generati dall'utente.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Indica se i dati nel controllo sono bloccati per la modifica.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| [IsTiled](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/istiled/) { get; set; } | Indica se l'immagine è ripetuta sullo sfondo. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Indica se il controllo è trasparente.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indica se questo controllo è visibile.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Ottiene e imposta la cella collegata.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Ottiene e imposta l'intervallo di riempimento dell'elenco.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Ottiene e imposta un'icona personalizzata da visualizzare come puntatore del mouse per il controllo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Ottiene e imposta il tipo di icona visualizzata come puntatore del mouse per il controllo.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Picture](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/picture/) { get; set; } | Ottiene e imposta i dati dell'immagine. |
| [PictureAlignment](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturealignment/) { get; set; } | Ottiene e imposta l'allineamento dell'immagine all'interno del Form o dell'Image. |
| [PictureSizeMode](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturesizemode/) { get; set; } | Ottiene e imposta come visualizzare l'immagine. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indica se mostrare un'ombra.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [SpecialEffect](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/specialeffect/) { get; set; } | Ottiene e imposta l'effetto speciale del controllo. |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Rappresenta come allineare il testo usato dal controllo.(Ereditato da [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/type/) { get; } | Ottiene il tipo del controllo ActiveX. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Ottiene e imposta la larghezza del controllo in unità di punti.(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Ottiene l'oggetto [`Workbook`](../activexcontrolbase/workbook/).(Ereditato da [`ActiveXControlBase`](../activexcontrolbase/).) |

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
using System.IO;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlDemo
    {
        public static void RunDemo()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo Image ActiveX al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 0, 1, 1, 100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà per il controllo Image ActiveX
            imageControl.IsAutoSize = true;
            imageControl.BorderOleColor = 0x000000; // Black border
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            imageControl.SpecialEffect = ControlSpecialEffectType.Flat;
            imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
            imageControl.IsTiled = false;

            // Carica un'immagine da file e impostala sul controllo
            byte[] imageData = File.ReadAllBytes("ImageActiveXControlDemo.jpg");
            imageControl.Picture = imageData;

            // Salva la cartella di lavoro
            workbook.Save("ImageActiveXControlDemo.xlsx");
            workbook.Save("ImageActiveXControlDemo.pdf");

            // Restituisci i risultati
            Console.WriteLine("Image ActiveX Control added with the following properties:");
            Console.WriteLine($"IsAutoSize: {imageControl.IsAutoSize}");
            Console.WriteLine($"BorderOleColor: {imageControl.BorderOleColor}");
            Console.WriteLine($"BorderStyle: {imageControl.BorderStyle}");
            Console.WriteLine($"PictureSizeMode: {imageControl.PictureSizeMode}");
            Console.WriteLine($"SpecialEffect: {imageControl.SpecialEffect}");
            Console.WriteLine($"PictureAlignment: {imageControl.PictureAlignment}");
            Console.WriteLine($"IsTiled: {imageControl.IsTiled}");
        }
    }
}
```

### Vedi anche

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


