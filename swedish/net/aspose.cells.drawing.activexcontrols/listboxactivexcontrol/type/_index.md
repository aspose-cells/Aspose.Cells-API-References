---
title: "ListBoxActiveXControl.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBoxActiveXControl egenskap. Hämtar typen av ActiveX-kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/type/
---
## ListBoxActiveXControl.Type property

Hämtar typen av ActiveX-kontrollen.

```csharp
public override ControlType Type { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en ListBox ActiveX-kontroll med alla nödvändiga parametrar
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 100, 100, 0, 0);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;
            
            // Demonstrera egenskapen Type
            Console.WriteLine("Control Type: " + listBox.Type);
            
            // Ställ in några egenskaper
            listBox.ScrollBars = ControlScrollBarType.BarsBoth;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter;
            listBox.ListStyle = ControlListStyle.Plain;
            listBox.SelectionType = SelectionType.Single;
            
            // Verifiera Type-egenskapen
            if (listBox.Type == ControlType.ListBox)
            {
                Console.WriteLine("This is a ListBox control as expected");
            }
            
            // Spara arbetsboken
            workbook.Save("ListBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ControlType](../../controltype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


