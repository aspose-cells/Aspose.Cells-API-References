---
title: "ComboBox.SelectedValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ComboBox. Ottiene il valore selezionato della casella combinata"
type: docs
url: /it/net/aspose.cells.drawing/combobox/selectedvalue/
---
## ComboBox.SelectedValue property

Ottiene il valore selezionato della casella combinata.

```csharp
public string SelectedValue { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertySelectedValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un ComboBox e aggiungi elementi
            Aspose.Cells.Drawing.ComboBox comboBox = (Aspose.Cells.Drawing.ComboBox)worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 50);
            comboBox.LinkedCell = "A1";
            comboBox.SetInputRange("B1:B4", false, false);
            
            // Imposta i valori nell'intervallo di input
            worksheet.Cells["B1"].PutValue("a");
            worksheet.Cells["B2"].PutValue("b");
            worksheet.Cells["B3"].PutValue("c");
            worksheet.Cells["B4"].PutValue("d");

            // Dimostra SelectedValue (proprietà di sola lettura)
            Console.WriteLine("SelectedValue: " + comboBox.SelectedValue);

            // Salva la cartella di lavoro
            workbook.Save("ComboBoxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


