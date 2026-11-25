---
title: "ComboBoxActiveXControl.IsDragBehaviorEnabled"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ComboBoxActiveXControl. Indica se il trascinamento e il rilascio sono abilitati per il controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/isdragbehaviorenabled/
---
## ComboBoxActiveXControl.IsDragBehaviorEnabled property

Indica se il trascinamento e il rilascio sono abilitati per il controllo.

```csharp
public bool IsDragBehaviorEnabled { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsDragBehaviorEnabledDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX ComboBox
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Imposta alcune proprietà di base
            comboBox.ListRows = 8;
            comboBox.ColumnCount = 1;
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = -1;

            // Dimostra la proprietà IsDragBehaviorEnabled
            Console.WriteLine("Initial IsDragBehaviorEnabled: " + comboBox.IsDragBehaviorEnabled);
            
            // Disabilita il comportamento di trascinamento
            comboBox.IsDragBehaviorEnabled = false;
            Console.WriteLine("After setting to false: " + comboBox.IsDragBehaviorEnabled);
            
            // Abilita il comportamento di trascinamento
            comboBox.IsDragBehaviorEnabled = true;
            Console.WriteLine("After setting to true: " + comboBox.IsDragBehaviorEnabled);

            // Salva la cartella di lavoro
            workbook.Save("ComboBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


