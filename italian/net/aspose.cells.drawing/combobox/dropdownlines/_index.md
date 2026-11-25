---
title: "ComboBox.DropDownLines"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ComboBox. Ottiene o imposta il numero di righe dell'elenco visualizzate nella parte a discesa di una casella combinata"
type: docs
url: /it/net/aspose.cells.drawing/combobox/dropdownlines/
---
## ComboBox.DropDownLines property

Ottiene o imposta il numero di righe della lista visualizzate nella parte a discesa di una casella combinata.

```csharp
public int DropDownLines { get; set; }
```

### Esempi

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertyDropDownLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una ComboBox con i parametri corretti
            ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 0, 0, 100, 100);
            comboBox.DropDownLines = 5;
            
            // Popola le celle del foglio di lavoro con gli elementi
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");
            worksheet.Cells["A6"].PutValue("Item 6");

            // Collega la casella combinata ai valori delle celle
            comboBox.InputRange = "A1:A6";

            workbook.Save("ComboBoxDropDownLinesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


