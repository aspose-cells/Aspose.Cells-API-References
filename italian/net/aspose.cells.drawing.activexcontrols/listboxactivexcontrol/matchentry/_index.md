---
title: "ListBoxActiveXControl.MatchEntry"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBoxActiveXControl. Indica come un ListBox o ComboBox ricerca la sua lista mentre l'utente digita"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/matchentry/
---
## ListBoxActiveXControl.MatchEntry property

Indica come un ListBox o ComboBox ricerca l'elenco mentre l'utente digita.

```csharp
public ControlMatchEntryType MatchEntry { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyMatchEntryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["A5"].PutValue("Date");

            // Aggiungi il controllo ListBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 1, 0, 100, 80);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Configura le proprietà del ListBox
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter;
            listBox.Value = "Apple;Banana;Cherry;Date";

            // Salva la cartella di lavoro
            workbook.Save("ListBoxMatchEntryDemo.xlsx");

            Console.WriteLine("ListBox with FirstLetter MatchEntry created successfully.");
        }
    }
}
```

### Vedi anche

* enum [ControlMatchEntryType](../../controlmatchentrytype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


