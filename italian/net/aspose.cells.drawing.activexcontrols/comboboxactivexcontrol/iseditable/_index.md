---
title: "ComboBoxActiveXControl.IsEditable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ComboBoxActiveXControl property. Indica se l'utente può digitare nel controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/iseditable/
---
## ComboBoxActiveXControl.IsEditable property

Indica se l'utente può digitare nel controllo.

```csharp
public bool IsEditable { get; set; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi un controllo ComboBox ActiveX usando la collezione Shapes
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 5, 0, 100, 30);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Imposta le proprietà per il ComboBox
            comboBox.IsEditable = true;
            comboBox.Value = "Editable ComboBox";
            comboBox.ColumnCount = 2;
            comboBox.ListRows = 6;
            comboBox.TextColumn = 1;

            // Aggiungi elementi al ComboBox (usando la proprietà ListFillRange)
            sheet.Cells["A10"].PutValue("Item 1");
            sheet.Cells["B10"].PutValue("Description 1");
            sheet.Cells["A11"].PutValue("Item 2");
            sheet.Cells["B11"].PutValue("Description 2");
            comboBox.ListFillRange = "A10:B11";

            // Salva la cartella di lavoro
            workbook.Save("ComboBoxActiveXControl_IsEditableDemo.xlsx");

            // Verifica la proprietà dopo il salvataggio
            Console.WriteLine("IsEditable property value: " + comboBox.IsEditable);
        }
    }
}
```

### Vedi anche

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


