---
title: "ActiveXControlBase.Data"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ActiveXControlBase. Ottiene e imposta i dati binari del controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/data/
---
## ActiveXControlBase.Data property

Ottiene e imposta i dati binari del controllo.

```csharp
public virtual byte[] Data { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;
    using System.Drawing;

    public class ActiveXControlBasePropertyDataDemo
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

            // Visualizza le informazioni iniziali della proprietà Data
            Console.WriteLine("Initial Data length: " + list.Data.Length);

            // Modifica le proprietà del controllo che influenzano Data
            list.BackOleColor = 0xFF0000;

            // Visualizza le informazioni aggiornate della proprietà Data
            Console.WriteLine("Modified Data length: " + list.Data.Length);

            // Salva la cartella di lavoro per dimostrare le modifiche persistenti
            workbook.Save("ActiveXControlDataDemo.xlsx");

        }
    }
}
```

### Vedi anche

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


