---
title: "Enum ControlMousePointerType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlMousePointerType enum. Rappresenta il tipo di icona visualizzata come puntatore del mouse per il controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/controlmousepointertype/
---
## ControlMousePointerType enumeration

Rappresenta il tipo di icona visualizzata come puntatore del mouse per il controllo.

```csharp
public enum ControlMousePointerType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Default | `0` | Puntatore standard. |
| Arrow | `1` | Freccia. |
| Cross | `2` | Puntatore a mirino. |
| IBeam | `3` | Cursore a forma di I. |
| SizeNESW | `6` | Doppia freccia che punta a nord-est e sud-ovest. |
| SizeNS | `7` | Doppia freccia che punta a nord e sud. |
| SizeNWSE | `8` | Doppia freccia che punta a nord-ovest e sud-est. |
| SizeWE | `9` | Doppia freccia che punta a ovest e est. |
| UpArrow | `10` | Freccia verso l'alto. |
| HourGlass | `11` | Clessidra. |
| NoDrop | `12` | Simbolo \"Not\" (cerchio con una linea diagonale) sopra l'oggetto trascinato. |
| AppStarting | `13` | Freccia con una clessidra. |
| Help | `14` | Freccia con un punto interrogativo. |
| SizeAll | `15` | Cursore \"Size-all\" (frecce che puntano a nord, sud, est e ovest). |
| Custom | `99` | Utilizza l'icona specificata dalla proprietà MouseIcon. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlMousePointerTypeDemo
    {
        public static void ControlMousePointerTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl control = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Esegui il cast di ActiveXControl a ActiveXControlBase per accedere alle sue proprietà
            ActiveXControlBase controlBase = control as ActiveXControlBase;

            if (controlBase != null)
            {
                // Imposta il tipo di puntatore del mouse per il controllo
                controlBase.MousePointer = ControlMousePointerType.Cross;

                // Imposta altre proprietà per la dimostrazione
                controlBase.Width = 150;
                controlBase.Height = 50;
                controlBase.IsVisible = true;
                controlBase.Shadow = true;
                controlBase.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
                controlBase.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
            }

            // Salva la cartella di lavoro
            workbook.Save("ControlMousePointerTypeExample.xlsx");
            workbook.Save("ControlMousePointerTypeExample.pdf");

            // Restituisci il risultato
            Console.WriteLine("Workbook with ActiveX control and custom mouse pointer type saved as 'ControlMousePointerTypeExample.xlsx'.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


