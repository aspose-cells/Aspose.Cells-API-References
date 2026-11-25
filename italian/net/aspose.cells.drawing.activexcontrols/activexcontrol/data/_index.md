---
title: "ActiveXControl.Data"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ActiveXControl. Ottiene e imposta i dati binari del controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrol/data/
---
## ActiveXControl.Data property

Ottiene e imposta i dati binari del controllo.

```csharp
public override byte[] Data { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlPropertyDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            cells["A2"].Value = "Sales";
            cells["A3"].Value = "Finance";
            cells["A4"].Value = "MIS";
            cells["A5"].Value = "R&D";
            cells["A6"].Value = "Marketing";
            cells["A7"].Value = "HRA";

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 5, 0, 100, 200);
            shape.Name = "MyList";
            ListBoxActiveXControl list = (ListBoxActiveXControl)shape.ActiveXControl;

            list.ListFillRange = ("A3:A7");
            list.Value = ("Apple");
            list.LinkedCell = ("A1");
            list.ListStyle = (ControlListStyle.Option);
            list.SelectionType = (SelectionType.Multi);
            list.IsVisible = true;

            // Visualizza le informazioni iniziali della proprietà Data
            Console.WriteLine("Initial Data length: " + list.Data.Length);

            // Modifica le proprietà del controllo che influenzano Data
            list.BackOleColor = 0xFF0000; 
            list.ListWidth = 200; // Increase list width

            // Visualizza le informazioni aggiornate della proprietà Data
            Console.WriteLine("Modified Data length: " + list.Data.Length);

            workbook.Save("ActiveXControlPropertyDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


