---
title: "Enum ControlType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlType enum. Rappresenta tutti i tipi di controllo ActiveX"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/controltype/
---
## ControlType enumeration

Rappresenta tutti i tipi di controllo ActiveX.

```csharp
public enum ControlType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| CommandButton | `0` | Pulsante |
| ComboBox | `1` | ComboBox |
| CheckBox | `2` | CheckBox |
| ListBox | `3` | ListBox |
| TextBox | `4` | TextBox |
| SpinButton | `5` | Spinner |
| RadioButton | `6` | RadioButton |
| Label | `7` | Etichetta |
| Image | `8` | Immagine |
| ToggleButton | `9` | ToggleButton |
| ScrollBar | `10` | ScrollBar |
| BarCode | `11` | ScrollBar |
| Unknown | `12` | Sconosciuto |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlTypeDemo
    {
        public static void ControlTypeExample()
        {
            // Inizializza una nuova cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX CommandButton
            Shape commandButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 1, 0, 1, 0, 100, 30);
            ActiveXControl commandButtonControl = commandButtonShape.ActiveXControl;
            commandButtonControl.IsEnabled = true;
            commandButtonControl.IsVisible = true;

            // Aggiungi un controllo ActiveX ComboBox
            Shape comboBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 3, 0, 1, 0, 100, 30);
            ActiveXControl comboBoxControl = comboBoxShape.ActiveXControl;
            comboBoxControl.IsEnabled = true;
            comboBoxControl.IsVisible = true;

            // Aggiungi un controllo ActiveX CheckBox
            Shape checkBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 1, 0, 100, 30);
            ActiveXControl checkBoxControl = checkBoxShape.ActiveXControl;
            checkBoxControl.IsEnabled = true;
            checkBoxControl.IsVisible = true;

            // Aggiungi un controllo ActiveX ListBox
            Shape listBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 7, 0, 1, 0, 100, 30);
            ActiveXControl listBoxControl = listBoxShape.ActiveXControl;
            listBoxControl.IsEnabled = true;
            listBoxControl.IsVisible = true;

            // Aggiungi un controllo ActiveX TextBox
            Shape textBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 9, 0, 1, 0, 100, 30);
            ActiveXControl textBoxControl = textBoxShape.ActiveXControl;
            textBoxControl.IsEnabled = true;
            textBoxControl.IsVisible = true;

            // Aggiungi un controllo ActiveX SpinButton
            Shape spinButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 11, 0, 1, 0, 100, 30);
            ActiveXControl spinButtonControl = spinButtonShape.ActiveXControl;
            spinButtonControl.IsEnabled = true;
            spinButtonControl.IsVisible = true;

            // Aggiungi un controllo ActiveX RadioButton
            Shape radioButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.RadioButton, 13, 0, 1, 0, 100, 30);
            ActiveXControl radioButtonControl = radioButtonShape.ActiveXControl;
            radioButtonControl.IsEnabled = true;
            radioButtonControl.IsVisible = true;

            // Aggiungi un controllo ActiveX Label
            Shape labelShape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 15, 0, 1, 0, 100, 30);
            ActiveXControl labelControl = labelShape.ActiveXControl;
            labelControl.IsEnabled = true;
            labelControl.IsVisible = true;

            // Aggiungi un controllo ActiveX Image
            Shape imageShape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 17, 0, 1, 0, 100, 30);
            ActiveXControl imageControl = imageShape.ActiveXControl;
            imageControl.IsEnabled = true;
            imageControl.IsVisible = true;

            // Aggiungi un controllo ActiveX ToggleButton
            Shape toggleButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 19, 0, 1, 0, 100, 30);
            ActiveXControl toggleButtonControl = toggleButtonShape.ActiveXControl;
            toggleButtonControl.IsEnabled = true;
            toggleButtonControl.IsVisible = true;

            // Aggiungi un controllo ActiveX ScrollBar
            Shape scrollBarShape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 21, 0, 1, 0, 100, 30);
            ActiveXControl scrollBarControl = scrollBarShape.ActiveXControl;
            scrollBarControl.IsEnabled = true;
            scrollBarControl.IsVisible = true;
                       

            // Salva la cartella di lavoro
            workbook.Save("ControlTypeExample.xlsx");
            workbook.Save("ControlTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


