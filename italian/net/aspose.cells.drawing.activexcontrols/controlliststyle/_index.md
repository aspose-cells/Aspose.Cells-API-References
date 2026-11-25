---
title: "Enum ControlListStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlListStyle enum. Rappresenta l'aspetto visivo dell'elenco in un ListBox o ComboBox"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/controlliststyle/
---
## ControlListStyle enumeration

Rappresenta l'aspetto visivo dell'elenco in una ListBox o ComboBox.

```csharp
public enum ControlListStyle
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Plain | `0` | Visualizza un elenco in cui lo sfondo di un elemento è evidenziato quando viene selezionato. |
| Option | `1` | Visualizza un elenco in cui un pulsante di opzione o una casella di controllo accanto a ogni voce mostra lo stato di selezione di quell'elemento. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlListStyleDemo
    {
        public static void ControlListStyleExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["A4"].PutValue("Item 3");

            // Aggiungi un controllo ActiveX ComboBox al foglio di lavoro
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà per il ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 3;
            comboBox.ColumnCount = 1;
            comboBox.ListStyle = ControlListStyle.Plain; // Set the ListStyle to Plain

            // Aggiungi elementi al ComboBox
            comboBox.Value = "Item 1";
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = 1;

            // Aggiungi un controllo ActiveX ListBox al foglio di lavoro
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;

            // Imposta le proprietà per il ListBox
            listBox.ColumnCount = 1;
            listBox.ListStyle = ControlListStyle.Option; // Set the ListStyle to Option

            // Aggiungi elementi al ListBox
            listBox.Value = "Item 1";
            listBox.BoundColumn = 1;
            listBox.TextColumn = 1;

            // Salva la cartella di lavoro
            workbook.Save("ControlListStyleExample.xlsx");
            workbook.Save("ControlListStyleExample.pdf");

            // Restituisci i risultati
            Console.WriteLine("ComboBox ListStyle: " + comboBox.ListStyle);
            Console.WriteLine("ListBox ListStyle: " + listBox.ListStyle);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


