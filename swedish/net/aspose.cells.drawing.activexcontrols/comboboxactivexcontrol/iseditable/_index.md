---
title: "ComboBoxActiveXControl.IsEditable"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl property. Anger om användaren kan skriva i kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/iseditable/
---
## ComboBoxActiveXControl.IsEditable property

Indikerar om användaren kan skriva i kontrollen.

```csharp
public bool IsEditable { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsEditableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till en ComboBox ActiveX control med hjälp av Shapes-samlingen
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 5, 0, 100, 30);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Ange egenskaper för ComboBox
            comboBox.IsEditable = true;
            comboBox.Value = "Editable ComboBox";
            comboBox.ColumnCount = 2;
            comboBox.ListRows = 6;
            comboBox.TextColumn = 1;

            // Lägg till objekt i ComboBox (med ListFillRange property)
            sheet.Cells["A10"].PutValue("Item 1");
            sheet.Cells["B10"].PutValue("Description 1");
            sheet.Cells["A11"].PutValue("Item 2");
            sheet.Cells["B11"].PutValue("Description 2");
            comboBox.ListFillRange = "A10:B11";

            // Spara arbetsboken
            workbook.Save("ComboBoxActiveXControl_IsEditableDemo.xlsx");

            // Verifiera egenskap efter sparning
            Console.WriteLine("IsEditable property value: " + comboBox.IsEditable);
        }
    }
}
```

### Se även

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


