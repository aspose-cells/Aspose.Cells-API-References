---
title: "Enum ControlBorderType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlBorderType enum. Rappresenta il tipo di bordo del controllo ActiveX"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/controlbordertype/
---
## ControlBorderType enumeration

Rappresenta il tipo di bordo del controllo ActiveX.

```csharp
public enum ControlBorderType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessun bordo. |
| Single | `1` | La singola riga. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;

    public class ControlBorderTypeDemo
    {
        public static void ControlBorderTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ComboBox al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà per il controllo ActiveX ComboBox
            comboBox.MaxLength = 100;
            comboBox.ListWidth = 150;
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = 1;
            comboBox.ColumnCount = 1;
            comboBox.ListRows = 5;
            comboBox.MatchEntry = ControlMatchEntryType.Complete;
            comboBox.DropButtonStyle = DropButtonStyle.Arrow;
            comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Always;
            comboBox.ListStyle = ControlListStyle.Plain;
            comboBox.BorderStyle = ControlBorderType.Single; // Set border style to Single
            comboBox.BorderOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Black);
            comboBox.SpecialEffect = ControlSpecialEffectType.Flat;
            comboBox.IsEditable = true;
            comboBox.ShowColumnHeads = false;
            comboBox.IsDragBehaviorEnabled = false;
            comboBox.EnterFieldBehavior = true;
            comboBox.IsAutoWordSelected = false;
            comboBox.SelectionMargin = false;
            comboBox.Value = "Sample Text";
            comboBox.HideSelection = true;
            comboBox.ColumnWidths = 100;

            // Salva la cartella di lavoro
            workbook.Save("ControlBorderTypeExample.xlsx");
            workbook.Save("ControlBorderTypeExample.pdf");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


