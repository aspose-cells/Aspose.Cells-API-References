---
title: "ComboBoxActiveXControl.ListRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl-egenskap. Representerar det maximala antalet rader som ska visas i listan"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/listrows/
---
## ComboBoxActiveXControl.ListRows property

Representerar det maximala antalet rader som ska visas i listan.

```csharp
public int ListRows { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyListRowsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ComboBox ActiveX-kontroll med korrekta bredd-/höjdparametrar
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 10, 10, 150, 30, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Lägg till exempelobjekt i kombinationsrutan med hjälp av ListFillRange
            comboBox.ListFillRange = "A1:A7";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");
            worksheet.Cells["A6"].PutValue("Item 6");
            worksheet.Cells["A7"].PutValue("Item 7");

            // Ställ in egenskapen ListRows för att kontrollera synliga objekt i rullgardinsmenyn
            comboBox.ListRows = 4; // Only show 4 items at a time

            // Spara arbetsboken
            workbook.Save("ComboBoxListRowsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


