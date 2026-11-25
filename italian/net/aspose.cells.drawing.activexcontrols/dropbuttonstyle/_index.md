---
title: "Enum DropButtonStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.DropButtonStyle enum. Rappresenta il simbolo visualizzato sul pulsante a discesa"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/dropbuttonstyle/
---
## DropButtonStyle enumeration

Rappresenta il simbolo visualizzato sul pulsante a discesa.

```csharp
public enum DropButtonStyle
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Plain | `0` | Visualizza un pulsante senza simbolo. |
| Arrow | `1` | Visualizza un pulsante con una freccia verso il basso. |
| Ellipsis | `2` | Visualizza un pulsante con un'ellissi (...). |
| Reduce | `3` | Visualizza un pulsante con una linea orizzontale simile al carattere di sottolineatura. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class DropButtonStyleDemo
    {
        public static void DropButtonStyleExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ComboBox al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà per il ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.ColumnCount = 1;
            comboBox.DropButtonStyle = DropButtonStyle.Arrow; // Set the drop button style to Arrow

            // Aggiungi alcuni elementi al ComboBox
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            comboBox.ListFillRange = "A1:A4";

            // Salva la cartella di lavoro
            workbook.Save("DropButtonStyleExample.xlsx");
            workbook.Save("DropButtonStyleExample.pdf");

            // Restituisci il DropButtonStyle utilizzato
            Console.WriteLine("DropButtonStyle set to: " + comboBox.DropButtonStyle);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


