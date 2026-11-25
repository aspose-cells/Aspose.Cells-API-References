---
title: "RadioButton.GroupBox"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RadioButton. Ottiene il GroupBox che contiene questo RadioButton"
type: docs
url: /it/net/aspose.cells.drawing/radiobutton/groupbox/
---
## RadioButton.GroupBox property

Ottiene il GroupBox che contiene questo RadioButton.

```csharp
public GroupBox GroupBox { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class RadioButtonPropertyGroupBoxDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un GroupBox per contenere i RadioButton
            GroupBox groupBox = worksheet.Shapes.AddGroupBox(1, 0, 100, 200, 100, 200);
            groupBox.Name = "OptionsGroup";
            groupBox.Shadow = true;

            // Aggiungi i RadioButton al foglio di lavoro (ancora non nel GroupBox)
            RadioButton radioButton1 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 20, 100, 20, 100);
            RadioButton radioButton2 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 50, 100, 20, 100);

            // Visualizza i valori iniziali della proprietà GroupBox (dovrebbe essere null)
            Console.WriteLine("RadioButton1 GroupBox before grouping: " + (radioButton1.GroupBox == null ? "null" : radioButton1.GroupBox.Name));
            Console.WriteLine("RadioButton2 GroupBox before grouping: " + (radioButton2.GroupBox == null ? "null" : radioButton2.GroupBox.Name));

            // Aggiungi i RadioButton al GroupBox impostando la posizione
            radioButton1.Placement = PlacementType.FreeFloating;
            radioButton2.Placement = PlacementType.FreeFloating;

            // Sposta i RadioButton all'interno del GroupBox
            radioButton1.Top = groupBox.Top + 20;
            radioButton1.Left = groupBox.Left + 20;
            radioButton2.Top = groupBox.Top + 50;
            radioButton2.Left = groupBox.Left + 20;

            // Visualizza i valori della proprietà GroupBox dopo il raggruppamento
            Console.WriteLine("RadioButton1 GroupBox after grouping: " + radioButton1.GroupBox.Name);
            Console.WriteLine("RadioButton2 GroupBox after grouping: " + radioButton2.GroupBox.Name);

            // Dimostra il comportamento del gruppo
            radioButton1.IsChecked = true;
            Console.WriteLine("RadioButton1 checked state: " + radioButton1.IsChecked);
            Console.WriteLine("RadioButton2 checked state: " + radioButton2.IsChecked);

            // Salva il risultato
            workbook.Save("RadioButtonPropertyGroupBoxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GroupBox](../../groupbox/)
* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


