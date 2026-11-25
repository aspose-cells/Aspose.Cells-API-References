---
title: "ListBoxActiveXControl.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBoxActiveXControl. Ottiene il tipo del controllo ActiveX"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/type/
---
## ListBoxActiveXControl.Type property

Ottiene il tipo del controllo ActiveX.

```csharp
public override ControlType Type { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un controllo ListBox ActiveX con tutti i parametri richiesti
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 100, 100, 0, 0);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
            
            // Dimostra la proprietà Type
            Console.WriteLine("Control Type: " + listBox.Type);
            
            // Imposta alcune proprietà
            listBox.ScrollBars = ControlScrollBarType.BarsBoth;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter;
            listBox.ListStyle = ControlListStyle.Plain;
            listBox.SelectionType = SelectionType.Single;
            
            // Verifica la proprietà Type
            if (listBox.Type == ControlType.ListBox)
            {
                Console.WriteLine("This is a ListBox control as expected");
            }
            
            // Salva la cartella di lavoro
            workbook.Save("ListBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ControlType](../../controltype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


